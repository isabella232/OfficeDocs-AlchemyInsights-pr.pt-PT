---
title: Definições de políticas de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627585"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="708ca-102">Gerenciar políticas de reunião em equipes da Microsoft</span><span class="sxs-lookup"><span data-stu-id="708ca-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="708ca-103">As políticas de reunião são usadas para controlar os recursos disponíveis para atender os participantes para reuniões agendadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="708ca-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="708ca-104">Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipes (elas são rotuladas como "em breve" na documentação).</span><span class="sxs-lookup"><span data-stu-id="708ca-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="708ca-105">Neste caso, ou se você está recebendo um erro como "Não podemos atualizar a política agora, mas experimentá-lo novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as políticas de reunião das equipes.</span><span class="sxs-lookup"><span data-stu-id="708ca-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="708ca-106">Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="708ca-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="708ca-107">Para saber mais sobre a criação de políticas, fazer mudanças e atribuir os usuários à política, [consulte as políticas de reunião em equipes.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="708ca-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="708ca-108">Para fazer alterações de política usando cmdlets PowerShell, consulte [equipes PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="708ca-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="708ca-109">Você precisa usar o [módulo Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) para políticas de reunião de equipes.</span><span class="sxs-lookup"><span data-stu-id="708ca-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="708ca-110">Analise a [documentação de cmdlets \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="708ca-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="708ca-111">**Nota:** Pode levar até 24 horas para que as alterações de política entrem em vigor para os usuários.</span><span class="sxs-lookup"><span data-stu-id="708ca-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="708ca-112">Você pode não ser capaz de fazer alterações nas políticas recém-criadas imediatamente; espere 4 horas e tente modificar uma política recém-criada novamente.</span><span class="sxs-lookup"><span data-stu-id="708ca-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="708ca-113">Se você ainda está tendo problemas, tente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="708ca-113">If you're still having problems, try PowerShell.</span></span>  