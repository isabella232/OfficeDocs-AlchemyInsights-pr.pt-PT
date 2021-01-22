---
title: Ligue a tecnologia NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935135"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="b3f8d-102">Ligue a tecnologia NDI</span><span class="sxs-lookup"><span data-stu-id="b3f8d-102">Turn on NDI technology</span></span>

<span data-ttu-id="b3f8d-103">A tecnologia NDI requer dois passos para ser ligado para um utilizador:</span><span class="sxs-lookup"><span data-stu-id="b3f8d-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="b3f8d-104">O administrador do arrendatário deve permitir a propriedade 'AllowNDIStreaming' em CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="b3f8d-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="b3f8d-105">Após esta alteração ter sido preenchida, o utilizador final deve ligar a tecnologia NDI® para o seu cliente específico a partir de **Definições > Permissões**.</span><span class="sxs-lookup"><span data-stu-id="b3f8d-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="b3f8d-106">Para obter mais informações, consulte [a tecnologia NDI em Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="b3f8d-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
