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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654267"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="e8154-102">Controlar as configurações do lobby e o nível de participação</span><span class="sxs-lookup"><span data-stu-id="e8154-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="e8154-103">Se você quiser permitir que todos, incluindo usuários discados, externos e anônimos, ignorem o lobby, você pode usar o PowerShell para fazê-lo.</span><span class="sxs-lookup"><span data-stu-id="e8154-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="e8154-104">Aqui está um exemplo de modificação da política de reunião global para sua organização:</span><span class="sxs-lookup"><span data-stu-id="e8154-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="e8154-105">Este cmdlet atualmente requer o uso do módulo Skype for Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e8154-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="e8154-106">Para obter configuração para usar este cmdlet, confira as políticas de [gestão via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="e8154-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="e8154-107">Você pode configurar uma nova política, que você precisará aplicá-la aos usuários.</span><span class="sxs-lookup"><span data-stu-id="e8154-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="e8154-108">Se você modificar a política global, ela se aplicará automaticamente aos usuários.</span><span class="sxs-lookup"><span data-stu-id="e8154-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="e8154-109">Para qualquer mudança de política, você precisa esperar pelo menos 4 horas e até 24 horas para que as políticas entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="e8154-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="e8154-110">Certifique-se de rever a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.</span><span class="sxs-lookup"><span data-stu-id="e8154-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="e8154-111">Entendendo equipes que aduntem controles de política saqueados do lobby</span><span class="sxs-lookup"><span data-stu-id="e8154-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="e8154-112">[Admitir automaticamente que as pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) são uma política por organizador que controla se as pessoas participam diretamente de uma reunião ou esperam no saguão até que sejam admitidas por um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="e8154-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="e8154-113">[Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem participar da reunião do usuário sem um usuário autenticado da organização presente.</span><span class="sxs-lookup"><span data-stu-id="e8154-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="e8154-114">[Permitir que os usuários dial-in para contornar o lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(em breve)** é uma política por organizador que controla se as pessoas que discar por telefone participar da reunião diretamente ou esperar no lobby, independentemente da configuração de **pessoas automaticamente admitir.**</span><span class="sxs-lookup"><span data-stu-id="e8154-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="e8154-115">[Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(em breve)** é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definido em **admitir automaticamente as pessoas** e permitir **dial-in usuários para contornar o lobby** quando eles agendar uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="e8154-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="e8154-116">**Nota:** Leia as políticas de [reunião gerenciadas em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para uma visão geral completa das políticas de reunião do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e8154-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
