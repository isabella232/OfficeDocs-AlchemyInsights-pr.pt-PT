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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376777"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="e85b4-102">Controle as configurações do lobby e nível de participação</span><span class="sxs-lookup"><span data-stu-id="e85b4-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="e85b4-103">Essas configurações controlam quais participantes da reunião esperam no lobby antes de serem admitidos na reunião e o nível de participação que são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e85b4-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="e85b4-104">Você pode usar o PowerShell para atualizar as configurações de diretiva de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração de equipes.</span><span class="sxs-lookup"><span data-stu-id="e85b4-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="e85b4-105">Veja abaixo um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.</span><span class="sxs-lookup"><span data-stu-id="e85b4-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="e85b4-106">[Admitir automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) que as pessoas são uma política por organizador que controla se as pessoas ingressem diretamente em uma reunião ou aguardem no lobby até que sejam admitidas por um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="e85b4-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e85b4-107">[Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem ingressar na reunião do usuário sem um usuário autenticado da organização no atendimento.</span><span class="sxs-lookup"><span data-stu-id="e85b4-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e85b4-108">[Permitir que os usuários de discagem ignorem o lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (em**breve**) é uma política por organizador que controla se as pessoas que discar por telefone ingressar na reunião diretamente ou aguardar no lobby, independentemente da configuração de **pessoas automaticamente admitir** .</span><span class="sxs-lookup"><span data-stu-id="e85b4-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e85b4-109">[Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**em breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definir em **admitir automaticamente as pessoas** e **permitir discagem usuários para ignorar o lobby** quando eles agendar uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="e85b4-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e85b4-110">**Nota:** Leia [gerenciar diretivas de reunião em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das diretivas de reunião do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e85b4-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="e85b4-111">**Exemplo do PowerShell**</span><span class="sxs-lookup"><span data-stu-id="e85b4-111">**PowerShell example**</span></span>

<span data-ttu-id="e85b4-112">Se você quiser permitir que todos, incluindo usuários externos ou anônimos, ignorem o lobby, você também pode usar o PowerShell para realizar essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="e85b4-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="e85b4-113">Veja um exemplo de como modificar a política de reunião global para sua organização.</span><span class="sxs-lookup"><span data-stu-id="e85b4-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="e85b4-114">(Certifique-se de rever a documentação acima antes de fazer essas alterações para entender exatamente o que isso permite.)</span><span class="sxs-lookup"><span data-stu-id="e85b4-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="e85b4-115">Set-CsTeamsMeetingPolicy-Identity global-Autoadmitedusers "Everyone"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="e85b4-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="e85b4-116">Para obter mais informações, consulte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="e85b4-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
