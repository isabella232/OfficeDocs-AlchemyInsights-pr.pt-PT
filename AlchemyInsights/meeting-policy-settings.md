---
title: Definições de política de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704617"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="af86a-102">Gerir políticas de reunião em Equipas da Microsoft</span><span class="sxs-lookup"><span data-stu-id="af86a-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="af86a-103">**Nota: Pode levar até 24 horas para que as alterações de política entrem em vigor para os utilizadores.**</span><span class="sxs-lookup"><span data-stu-id="af86a-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="af86a-104">Pode não ser capaz de fazer alterações às políticas recém-criadas imediatamente; aguarde 4 horas e tente modificar uma política recém-criada novamente.</span><span class="sxs-lookup"><span data-stu-id="af86a-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="af86a-105">As políticas de reunião são usadas para controlar as funcionalidades disponíveis para reunir os participantes para reuniões que são agendadas pelos utilizadores da sua organização.</span><span class="sxs-lookup"><span data-stu-id="af86a-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="af86a-106">Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipas (estas estão rotuladas "em breve" na documentação).</span><span class="sxs-lookup"><span data-stu-id="af86a-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="af86a-107">Neste caso, ou se estiver a obter um erro como "Não podemos atualizar a política neste momento, mas tente novamente mais tarde" no centro de administração da Microsoft Teams, recomendamos que utilize o PowerShell para criar ou modificar as políticas de reunião de Equipas.</span><span class="sxs-lookup"><span data-stu-id="af86a-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="af86a-108">Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="af86a-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="af86a-109">Para aprender a criar políticas, a fazer alterações e a atribuir os utilizadores à política, consulte [Gerir políticas de reunião em Equipas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="af86a-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="af86a-110">Para escoar alterações de política utilizando cmdlets PowerShell, consulte [a Visão Geral do PowerShell das Equipas](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="af86a-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="af86a-111">Você precisa usar o [módulo Skype para Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) para equipas que cumprem políticas.</span><span class="sxs-lookup"><span data-stu-id="af86a-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="af86a-112">Reveja a [documentação dos cmdlets da \*-CSTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="af86a-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

