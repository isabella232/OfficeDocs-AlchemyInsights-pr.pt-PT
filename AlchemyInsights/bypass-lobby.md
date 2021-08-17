---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059607"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlar as definições da sala de espera e o nível de participação Teams

Se quiser permitir que todas as pessoas, incluindo utilizadores **externos, externos** e anónimos, entrem sem passar pela sala de espera , utilize o PowerShell para realizar esta tarefa. Eis um exemplo de como modificar a política de reunião global para a sua organização.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Neste momento, este cmdlet necessita da utilização Skype para Empresas módulo do PowerShell. Para configurar para utilizar este cmdlet, consulte Gerir [políticas através do PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Depois de configurar uma política, tem de aplicá-la aos utilizadores; ou, se tiver modificado a Política global, a mesma será aplicada automaticamente aos utilizadores. Para qualquer alteração de política, tem de esperar, pelo menos, 4 horas até **24 horas** para que as políticas entrem em vigor. 

Certifique-se de que revê a documentação abaixo antes de fazer estas alterações para compreender exatamente o que isto permite.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Compreender os Teams de sala de espera de reuniões

Estas definições controlam que participantes da reunião aguardam na sala de espera antes de entrarem na reunião e o nível de participação que podem participar numa reunião. Pode utilizar o PowerShell para atualizar as definições da política de reunião que ainda não foram implementadas (indique "brevemente") no centro de administração do Teams reunião. Consulte abaixo um cmdlet do PowerShell de exemplo que permite que todos os utilizadores entrem sem passar pela sala de espera.

- [Admitir automaticamente as pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas entram diretamente numa reunião ou aguardam na sala de espera até que sejam admitidas por um utilizador autenticado.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Permitir que pessoas anónimas iniciem uma reunião é uma política por organizador que controla se as pessoas anónimas, incluindo B2B e utilizadores federados, podem participar na reunião do utilizador sem que um utilizador autenticado da organização participe.

- Permitir que os utilizadores de acesso telefónico entrem diretamente na sala de espera (brevemente) é uma política por organizador que controla se as pessoas que ligam por telefone entram diretamente na reunião ou esperam na sala de espera, independentemente da definição Admitir pessoas automaticamente. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)  

- Permitir que os organizadores definam as definições da sala de espera (brevemente) é uma política por organizador que controla se  o organizador da reunião pode desativar as definições da sala de espera definidas por um administrador em Admitir automaticamente pessoas e Permitir que os utilizadores de acesso teleguizado entrem sem passar pela sala de espera quando agendam uma nova reunião. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)  

**Nota:** Leia [Gerir políticas de reunião Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para uma visão geral completa das Microsoft Teams de reuniões.
