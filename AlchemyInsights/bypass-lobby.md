---
title: Lobby de desvio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889093"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controle as configurações do lobby e o nível de participação em equipes

Se você quiser permitir que todos, incluindo usuários discados, externos e anônimos, **ignorem o lobby,** use o PowerShell para realizar essa tarefa. Aqui está um exemplo de modificação da política de reunião global para sua organização.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Este cmdlet atualmente requer o uso do módulo Skype for Business PowerShell. Para ser configurado para usar este cmdlet, confira as políticas de [gestão via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Depois de configurar uma política, você precisa aplicá-la aos usuários; ou, se você modificou a política global, ela será aplicada automaticamente aos usuários. Para qualquer mudança de política, você precisa esperar pelo menos **4 horas até 24 horas** para que as políticas entrem em vigor. 

Certifique-se de rever a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Entendendo equipes que aduntem controles de política saqueados do lobby

Essas configurações controlam qual reunião os participantes aguardam no saguão antes de serem admitidos na reunião e o nível de participação permitidos em uma reunião. Você pode usar o PowerShell para atualizar as configurações de política de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração das Equipes. Veja abaixo um exemplo powershell cmdlet que permite que todos os usuários para contornar o lobby.

- [Admitir automaticamente que as pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) são uma política por organizador que controla se as pessoas participam diretamente de uma reunião ou esperam no saguão até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem participar da reunião do usuário sem um usuário autenticado da organização presente.

- [Permitir que os usuários dial-in para contornar o lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(em breve)** é uma política por organizador que controla se as pessoas que discar por telefone participar da reunião diretamente ou esperar no lobby, independentemente da configuração de **pessoas automaticamente admitir.**

- [Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(em breve)** é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definido em **automaticamente admitir pessoas** e permitir que os **usuários dial-in para contornar o lobby** quando eles agendar uma nova reunião.

**Nota:** Leia as políticas de [reunião gerenciadas em equipes](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para uma visão geral completa das políticas de reunião do Microsoft Teams.
