---
title: Remoção do problema PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972727"
---
# <a name="troubleshoot-prt-issue"></a>Remoção do problema PRT

Para que qualquer dispositivo conclua a autenticação, tem de estar totalmente registado e em bom estado e conseguir adquirir um Token de Atualização Principal (PRT).

O processo de registo de associação do Azure AD híbrido requer que os dispositivos estejam numa rede empresarial. Também funciona com VPN, mas existem algumas ressaltas para isso. Ouvimos os clientes que precisam de assistência para resolver o processo de registo híbrido do Azure AD em circunstâncias de trabalho remoto. Eis uma discriminação do que está a acontecer durante o processo de registo.

**Ambiente de autenticação na nuvem (com sincronização de hashes de palavras-passe do Azure AD ou autenticação pass-through)**

Este fluxo de registo também é conhecido como "Associação de Sincronização".

1. Windows 10 deteta um registo SCP após o utilizador ter a oportunidade de o fazer no dispositivo.
    1. O dispositivo tenta primeiro obter informações do inquilino do SCP do lado do cliente no registo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obter mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Se falhar, o dispositivo comunica com o Active Directory (AD) no local para obter informações do inquilino através do Service Connection Point (SCP). Para verificar o SCP, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Recomendamos que ativar o SCP no AD e utilizar apenas o SCP do lado do cliente para validação inicial.

2. Windows 10 a comunicar com o Azure AD no contexto do sistema para se autenticar contra o Azure AD. Pode verificar se o dispositivo pode aceder aos recursos da Microsoft na conta do sistema através do script de Conectividade de Registo de Dispositivos de Teste.

3. Windows 10 gera um certificado autoassinado e armazena-o no objeto do computador no AD no local. Isto requer que o Controlador de Domínios exija que o Controlador de Domínios o desloquem.

4. Um objeto de dispositivo com um certificado é sincronizado com o Azure AD através do Azure AD Ligação. Por predefinição, o ciclo de sincronização é a cada 30 minutos, mas depende da configuração do Azure AD Ligação. Para obter mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Nesta fase, deverá conseguir ver o dispositivo com o assunto no estado "Pendente" em Dispositivo com o dispositivo do Portal do Azure.

6. Na próxima sessão de início de sessão Windows 10 utilizador, o registo será concluído. 

> [!NOTE]
> Se estiver a usar VPN e um processo de início de sessão com logótipo terminar a conectividade do domínio, pode ativar o registo manualmente:
 1. Emite um dsregcmd /join localmente numa mensagem de administração ou remotamente através do PSExec para o seu PC. Por exemplo, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Para obter mais detalhes sobre problemas de Associação Híbrida, [consulte Remoção de problemas de dispositivos.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
