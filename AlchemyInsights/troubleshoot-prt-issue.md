---
title: Problema de resolução de problemas prt
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573723"
---
# <a name="troubleshoot-prt-issue"></a>Problema de resolução de problemas prt

Para que qualquer dispositivo complete a autenticação, deve estar totalmente registado e em bom estado e capaz de adquirir um Token Primary Refresh (PRT).

O processo híbrido Azure AD junta-se ao processo de registo requer que os dispositivos estejam numa rede corporativa. Também funciona sobre a VPN, mas há algumas ressalvas nisso. Ouvimos clientes que precisam de ajuda para resolver problemas com o híbrido Azure AD aderir ao processo de registo em circunstâncias de trabalho remoto. Aqui está uma descrição do que está a acontecer 'debaixo do capot' durante o processo de registo.

**Ambiente de autenticação em nuvem (utilizando a sincronização de haxixe de palavra-passe AZure ou a autenticação de passagem)**

Este fluxo de registo também é conhecido como "Sync Join".

1. O Windows 10 descobre um registo SCP ao iniciar sessão no dispositivo.
    1. O dispositivo tenta primeiro obter informações do cliente da SCP do lado do cliente no registo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Se falhar, o dispositivo comunica com o Ative Directory (AD) no local para obter informações do inquilino do Ponto de Ligação de Serviço (SCP). Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Recomendamos que se habilita o SCP no AD e utilize apenas o SCP do lado do cliente para validação inicial.

2. O Windows 10 tenta comunicar com o Azure AD no contexto do sistema para se autenticar contra o AD Azure. Pode verificar se o dispositivo pode aceder aos recursos da Microsoft sob a conta do sistema utilizando o script de conectividade de registo do dispositivo de teste.

3. O Windows 10 gera um certificado auto-assinado e armazena-o sob o objeto do computador no Local AD. Isto requer uma linha de visão para o Controlador de Domínio.

4. Um objeto do dispositivo que tenha um certificado é sincronizado com a Azure AD via Azure AD Connect. O ciclo de sincronização é a cada 30 minutos por defeito, mas depende da configuração do Azure AD Connect. Para mais informações, por favor leia as referências a este [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Nesta fase, deverá ser possível ver o dispositivo do sujeito em estado "Pendente" sob a lâmina do Dispositivo do Portal Azure.

6. No próximo login do utilizador para o Windows 10, o registo será concluído. 

> [!NOTE]
> Se estiver na VPN e um processo de login de logoff terminar a conectividade do domínio, pode acionar o registo manualmente:
 1. Emita um dsregcmd /junte-se localmente na solicitação de administração ou remotamente através do PSExec para o seu PC. Por exemplo, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Para obter mais detalhes sobre os problemas da Hybrid Join, consulte [a Questão dos dispositivos de resolução de problemas](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
