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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768451"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Controlar as configurações do lobby e o nível de participação

Se você quiser permitir que todos, incluindo usuários discados, externos e anônimos, ignorem o lobby do Microsoft Teams, você pode usar o PowerShell para fazê-lo. Aqui está um exemplo de modificação da política de reunião global para sua organização:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Este cmdlet atualmente requer o uso do módulo Skype for Business PowerShell. Para obter configuração para usar este cmdlet, confira as políticas de [gestão via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Você pode configurar uma nova política, que você precisará aplicá-la aos usuários. Se você modificar a política global, ela se aplicará automaticamente aos usuários. Para qualquer mudança de política, você precisa esperar pelo menos 4 horas e até 24 horas para que as políticas entrem em vigor.

Certifique-se de rever a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Entendendo equipes que aduntem controles de política saqueados do lobby

- [Admitir automaticamente que as pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) são uma política por organizador que controla se as pessoas participam diretamente de uma reunião ou esperam no saguão até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem participar da reunião do usuário sem um usuário autenticado da organização presente.

- [Permitir que os usuários dial-in para contornar o lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(em breve)** é uma política por organizador que controla se as pessoas que discar por telefone participar da reunião diretamente ou esperar no lobby, independentemente da configuração de **pessoas automaticamente admitir.**

- [Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(em breve)** é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definido em **automaticamente admitir pessoas** e permitir que os **usuários dial-in para contornar o lobby** quando eles agendar uma nova reunião.

**Nota:** Leia as políticas de [reunião gerenciadas em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para uma visão geral completa das políticas de reunião do Microsoft Teams.
