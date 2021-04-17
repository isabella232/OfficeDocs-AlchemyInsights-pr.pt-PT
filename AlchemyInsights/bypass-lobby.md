---
title: Lobby de bypass
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
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820045"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="7165a-102">Definições de lobby de controlo e nível de participação em equipas</span><span class="sxs-lookup"><span data-stu-id="7165a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="7165a-103">Se quiser permitir que todos, incluindo utilizadores de acesso de marcação, externos e anónimos, **contornem o lobby,** utilize o PowerShell para realizar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="7165a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="7165a-104">Aqui está um exemplo de modificar a política global de reuniões para a sua organização.</span><span class="sxs-lookup"><span data-stu-id="7165a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7165a-105">Este cmdlet requer atualmente a utilização do Módulo Skype para Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7165a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7165a-106">Para se preparar para utilizar este cmdlet, consulte [as políticas de gestão via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="7165a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7165a-107">Uma vez configurada uma política, tem de a aplicar aos utilizadores; ou, se modificar a política Global, aplicar-se-á automaticamente aos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="7165a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="7165a-108">Para qualquer mudança de política, é necessário esperar pelo menos **4 horas até 24 horas** para que as políticas entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="7165a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="7165a-109">Certifique-se de rever a documentação abaixo antes de então fazer estas alterações para entender exatamente o que isso permite.</span><span class="sxs-lookup"><span data-stu-id="7165a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7165a-110">Equipas compreensivas que reúnem controlos políticos de lobby</span><span class="sxs-lookup"><span data-stu-id="7165a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="7165a-111">Estas definições controlam quais os participantes que se encontram aguardam no átrio antes de serem admitidos na reunião e do nível de participação que lhes é permitido numa reunião.</span><span class="sxs-lookup"><span data-stu-id="7165a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7165a-112">Pode utilizar o PowerShell para atualizar as definições de política de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração das Equipas.</span><span class="sxs-lookup"><span data-stu-id="7165a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="7165a-113">Veja abaixo um exemplo PowerShell cmdlet que permite a todos os utilizadores contornar o lobby.</span><span class="sxs-lookup"><span data-stu-id="7165a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="7165a-114">[Admitir automaticamente as pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas se juntam a uma reunião diretamente ou esperam no lobby até serem admitidas por um utilizador autenticado.</span><span class="sxs-lookup"><span data-stu-id="7165a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7165a-115">[Permitir que pessoas anónimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anónimas, incluindo B2B e utilizadores federados, podem participar na reunião do utilizador sem um utilizador autenticado da organização presente.</span><span class="sxs-lookup"><span data-stu-id="7165a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7165a-116">[Permitir que os utilizadores de acesso telefónico contornem o lobby (em](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que ligam por telefone se juntam diretamente à reunião ou esperam no lobby **independentemente** da configuração automática de pessoas.</span><span class="sxs-lookup"><span data-stu-id="7165a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7165a-117">[Permitir que os organizadores substituam as definições de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(em breve**) é uma política por organizador que controla se o organizador da reunião pode sobrepor as definições do lobby que um administrador definido em Automaticamente **admitem pessoas** e **permitem que os utilizadores de acesso de marcação contornem o lobby** quando agendam uma nova reunião.</span><span class="sxs-lookup"><span data-stu-id="7165a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7165a-118">**Nota:** Leia [Gerir as políticas de reunião em Equipas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para uma visão geral completa das políticas de reunião das Equipas da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7165a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
