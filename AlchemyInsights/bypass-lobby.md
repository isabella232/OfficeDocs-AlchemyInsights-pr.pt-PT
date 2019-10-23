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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="4e636-102">Controle as configurações do lobby e nível de participação</span><span class="sxs-lookup"><span data-stu-id="4e636-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="4e636-103">Se você quiser permitir que todos, incluindo usuários dial-in, externos e anônimos ignorem o lobby, você pode usar o PowerShell para fazê-lo.</span><span class="sxs-lookup"><span data-stu-id="4e636-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="4e636-104">Veja um exemplo de como modificar a política de reunião global para sua organização:</span><span class="sxs-lookup"><span data-stu-id="4e636-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="4e636-105">Atualmente, esse cmdlet requer o uso do módulo do PowerShell do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="4e636-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="4e636-106">Para obter a configuração para usar esse cmdlet, confira Gerenciando diretivas por meio do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4e636-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="4e636-107">Você pode configurar uma nova política, que precisará aplicá-la aos usuários.</span><span class="sxs-lookup"><span data-stu-id="4e636-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="4e636-108">Se você modificar a política global, ela será automaticamente aplicada aos usuários.</span><span class="sxs-lookup"><span data-stu-id="4e636-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="4e636-109">Para qualquer alteração de política, você precisa aguardar pelo menos 4 horas e até 24 horas para que as diretivas tenham efeito.</span><span class="sxs-lookup"><span data-stu-id="4e636-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="4e636-110">Certifique-se de rever a documentação abaixo antes de fazer essas alterações para entender exatamente o que isso permite.</span><span class="sxs-lookup"><span data-stu-id="4e636-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="4e636-111">Noções básicas sobre equipes reunião controles de diretiva de lobby</span><span class="sxs-lookup"><span data-stu-id="4e636-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="4e636-112">[Admitir automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) que as pessoas são uma política por organizador que controla se as pessoas ingressem diretamente em uma reunião ou aguardem no lobby até que sejam admitidas por um usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="4e636-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="4e636-113">[Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem ingressar na reunião do usuário sem um usuário autenticado da organização no atendimento.</span><span class="sxs-lookup"><span data-stu-id="4e636-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="4e636-114">[Permitir que os usuários de discagem ignorem o lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (em**breve**) é uma política por organizador que controla se as pessoas que discar por telefone ingressar na reunião diretamente ou aguardar no lobby, independentemente da configuração de **pessoas automaticamente admitir** .</span><span class="sxs-lookup"><span data-stu-id="4e636-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="4e636-115">[Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**em breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definir em **admitir automaticamente as pessoas** e **permitir discagem usuários para ignorar o lobby** quando eles agendar uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="4e636-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="4e636-116">**Nota:** Leia [gerenciar diretivas de reunião em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das diretivas de reunião do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4e636-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
