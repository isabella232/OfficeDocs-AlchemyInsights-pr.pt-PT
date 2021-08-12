---
title: Dispositivo em estado pendente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914014"
---
# <a name="device-in-pending-state"></a>Dispositivo em estado pendente

**Pré-requisitos:**

1. Se estiver a configurar registos de dispositivos pela primeira vez, certifique-se de que reviu a Introdução à gestão de dispositivos no [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) que irá guiá-lo sobre como colocar os dispositivos sob controlo do Azure AD.
2. Se estiver a registar dispositivos diretamente no Azure AD e a inscrever os [dispositivos](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) no Intune, terá de se certificar de que configurou o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e de que o licenciamento está em vigor primeiro.
3. Certifique-se de que está autorizado a efetuar operações no Azure AD e no AD no local. Apenas um administrador global no Azure AD pode gerir as definições dos registos de dispositivos. Além disso, se estiver a configurar o registo automático no seu Active Directory no local, terá de ser um administrador do Active Directory e do AD FS (se aplicável).

O processo de registo de associação do Azure AD híbrido exige que os dispositivos se encontrarem na rede empresarial. Também funciona com VPN, mas existem algumas ressaltas para isso. Ouvimos os clientes que precisam de assistência para resolver o processo de registo híbrido do Azure AD em circunstâncias de trabalho remoto.

**Ambiente de autenticação na nuvem (com sincronização de hashes de palavras-passe do Azure AD ou autenticação pass-through)**

Este fluxo de registo também é conhecido como "Associação de Sincronização".

Eis uma discriminação do que acontece durante o processo de registo:

1. Windows 10 deteta o registo do Ponto de Ligação de Serviço (SCP) quando o utilizador iniciar sessão no dispositivo.

    1. O dispositivo tenta primeiro obter informações do inquilino do SCP do lado do cliente no registo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obter mais informações, consulte [o documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Se falhar, o dispositivo comunica com o Active Directory no local para obter informações do inquilino através do SCP. Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Recomendamos a ativação do SCP no Active Directory e a utilização apenas do SCP do lado do cliente para validação inicial.

2. Windows 10 a comunicar com o Azure AD no contexto do sistema para se autenticar contra o Azure AD.

    Pode verificar se o dispositivo pode aceder aos recursos da Microsoft na conta do sistema ao utilizar o script de Conectividade [de Registo de Dispositivos de Teste.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 gera certificado autoassinado e armazena-o sob o objeto de computador no Active Directory no local. Isto requer que o Controlador de Domínios exija que o Controlador de Domínios o desloquem.

4. O objeto de dispositivo com o certificado é sincronizado com o Azure AD através do Azure AD Ligação. Por predefinição, o ciclo de sincronização é a cada 30 minutos, mas depende da configuração do Azure AD Ligação. Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Nesta fase, deverá conseguir ver o dispositivo com o assunto no estado "**Pendente**" em Dispositivo com o dispositivo do Portal do Azure.

6. Na próxima sessão de início de sessão Windows 10 utilizador, o registo será concluído.

    > [!NOTE]
    > Se estiver a usar VPN e o logótipo/início de sessão terminar a conectividade do domínio, pode ativar o registo manualmente. Para o fazer:
    >
    > Emite `dsregcmd /join` um problema localmente num pedido de administração ou remotamente através do PSExec para o seu PC.
    >
    > Por exemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Para problemas comuns com o Azure Active Directory de dispositivos, consulte as [FAQ dos Dispositivos.](https://docs.microsoft.com/azure/active-directory/devices/faq)
