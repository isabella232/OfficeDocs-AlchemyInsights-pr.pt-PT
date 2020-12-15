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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679988"
---
# <a name="device-in-pending-state"></a>Dispositivo em estado pendente

**Pré-requisitos:**

1. Se estiver a configurar os registos do dispositivo pela primeira vez, certifique-se de que reviu [a Introdução à gestão do dispositivo no Azure Ative Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) que o guiará sobre como obter dispositivos sob o controlo da Azure AD.
2. Se estiver a registar os dispositivos no Azure AD diretamente e a inscrevê-los no Intune, terá de se certificar de que [tem configurado Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e ter o [licenciamento](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) em primeiro lugar.
3. Certifique-se de que está autorizado a realizar operações em Azure AD e no local AD. Apenas um administrador global em Azure AD pode gerir as definições para registos de dispositivos. Além disso, se estiver a configurar registos automáticos no seu Ative Directory no local, terá de ser administrador do Ative Directory e da AD FS (se aplicável).

O processo híbrido Azure AD aderir ao processo de registo requer que os dispositivos estejam na rede corporativa. Também funciona sobre a VPN, mas há algumas ressalvas nisso. Ouvimos os clientes precisarem de assistência para resolver problemas com o híbrido Azure AD aderir ao processo de registo em circunstâncias de trabalho remoto.

**Ambiente de autenticação em nuvem (utilizando a sincronização de haxixe de palavra-passe AZure ou a autenticação de passagem)**

Este fluxo de registo também é conhecido como "Sync Join".

Aqui está uma descrição do que acontece durante o processo de registo:

1. O Windows 10 descobre o registo do Ponto de Ligação de Serviço (SCP) quando o utilizador inicia sessão no dispositivo.

    1. O dispositivo tenta primeiro obter informações do cliente da SCP do lado do cliente no registo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para mais informações, consulte [o documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Se falhar, o dispositivo comunica com o Ative Directory no local para obter informações do inquilino da SCP. Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Recomendamos que se habilita o SCP no Ative Directory e utilize apenas o SCP do lado do cliente para validação inicial.

2. O Windows 10 tenta comunicar com o Azure AD no contexto do sistema para se autenticar contra o AD Azure.

    Pode verificar se o dispositivo pode aceder aos recursos da Microsoft sob a conta do sistema utilizando o [script de conectividade de registo do dispositivo de teste](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. O Windows 10 gera certificado auto-assinado e armazena-o sob o objeto do computador no Ative Directory. Isto requer uma linha de visão para o Controlador de Domínio.

4. O objeto do dispositivo que tem certificado é sincronizado com Azure AD via Azure AD Connect. O ciclo de sincronização é a cada 30 minutos por defeito, mas depende da configuração do Azure AD Connect. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Nesta fase, você deve ser capaz de ver o dispositivo sujeito em estado "**Pendente**" sob a lâmina do dispositivo do Portal Azure.

6. No próximo login do utilizador para o Windows 10, o registo será concluído.

    > [!NOTE]
    > Se estiver em VPN e o logoff/login terminar a conectividade do domínio, pode ativar o registo manualmente. Para fazer isto:
    >
    > Emita um `dsregcmd /join` local local na solicitação de administração ou remotamente via PSExec para o seu PC.
    >
    > Por exemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Para questões comuns com o registo do dispositivo Azure Ative Directory, consulte [O FAQ dos Dispositivos](https://docs.microsoft.com/azure/active-directory/devices/faq).
