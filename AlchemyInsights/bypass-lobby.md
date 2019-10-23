---
title: Bypass lobby
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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637788"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Controle as configurações do lobby e nível de participação

Se você quiser permitir que todos, incluindo usuários dial-in, externos e anônimos ignorem o lobby, você pode usar o PowerShell para fazê-lo. Veja um exemplo de como modificar a política de reunião global para sua organização:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Atualmente, esse cmdlet requer o uso do módulo do PowerShell do Skype for Business. Para obter a configuração para usar esse cmdlet, confira Gerenciando diretivas por meio do PowerShell.

Você pode configurar uma nova política, que precisará aplicá-la aos usuários. Se você modificar a política global, ela será automaticamente aplicada aos usuários. Para qualquer alteração de política, você precisa aguardar pelo menos 4 horas e até 24 horas para que as diretivas tenham efeito.

Certifique-se de rever a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Noções básicas sobre equipes reunião controles de diretiva de lobby

- [Admitir automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) que as pessoas são uma política por organizador que controla se as pessoas ingressem diretamente em uma reunião ou aguardem no lobby até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem ingressar na reunião do usuário sem um usuário autenticado da organização no atendimento.

- [Permitir que os usuários de discagem ignorem o lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (em**breve**) é uma política por organizador que controla se as pessoas que discar por telefone ingressar na reunião diretamente ou aguardar no lobby, independentemente da configuração de **pessoas automaticamente admitir** .

- [Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**em breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definir em **admitir automaticamente as pessoas** e **permitir discagem usuários para ignorar o lobby** quando eles agendar uma nova reunião.

**Nota:** Leia [gerenciar diretivas de reunião em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das diretivas de reunião do Microsoft Teams.
