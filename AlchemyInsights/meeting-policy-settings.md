---
title: Definições políticas de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042855"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="3252f-102">Gerir as políticas de reunião em Equipas microsoft</span><span class="sxs-lookup"><span data-stu-id="3252f-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="3252f-103">**Nota: Pode levar até 24 horas para que as alterações de política entrem em vigor para os utilizadores.**</span><span class="sxs-lookup"><span data-stu-id="3252f-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="3252f-104">Pode não ser capaz de fazer alterações às políticas recém-criadas imediatamente; esperar 4 horas e tentar modificar uma política recém-criada novamente.</span><span class="sxs-lookup"><span data-stu-id="3252f-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="3252f-105">As políticas de reunião são usadas para controlar as funcionalidades que estão disponíveis para reunir os participantes para reuniões agendadas pelos utilizadores da sua organização.</span><span class="sxs-lookup"><span data-stu-id="3252f-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="3252f-106">Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipas (estas estão rotuladas como "em breve" na documentação).</span><span class="sxs-lookup"><span data-stu-id="3252f-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="3252f-107">Neste caso, ou se estiver a ter um erro como "Não podemos atualizar a apólice agora, mas tente novamente mais tarde" no centro de administração da Microsoft Teams, recomendamos que use o PowerShell para criar ou modificar as políticas de reunião das Equipas.</span><span class="sxs-lookup"><span data-stu-id="3252f-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="3252f-108">Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="3252f-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="3252f-109">Para aprender sobre a criação de políticas, fazer alterações e atribuir utilizadores à política, consulte [gerir as políticas de reunião em Equipas.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="3252f-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="3252f-110">Para fazer alterações de política utilizando cmdlets PowerShell, consulte a visão geral do [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="3252f-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="3252f-111">Você precisa usar o [módulo Skype para Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) para as políticas de reunião de equipas.</span><span class="sxs-lookup"><span data-stu-id="3252f-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="3252f-112">Reveja a [documentação de \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="3252f-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

