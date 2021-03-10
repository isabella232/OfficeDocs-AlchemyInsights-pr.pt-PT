---
title: Fixar regras de transporte
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695858"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="3876e-102">Fixar regras de transporte</span><span class="sxs-lookup"><span data-stu-id="3876e-102">Fix transport rules</span></span>

<span data-ttu-id="3876e-103">Uma regra de fluxo de correio personalizado afetou esta mensagem.</span><span class="sxs-lookup"><span data-stu-id="3876e-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="3876e-104">Para rever a regra exata, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="3876e-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="3876e-105">Nos resultados da submissão, em **informações adicionais,** note o **GUID** ou o **Nome De Política**.</span><span class="sxs-lookup"><span data-stu-id="3876e-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="3876e-106">Launch Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="3876e-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="3876e-107">Para mais informações, consulte [Abrir a Shell de Gestão de Câmbios.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="3876e-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="3876e-108">Executar este comando (utilizando o GUID a partir da sua submissão):  **Get-TransportRule -identidade "GUID" | fl \* Descrição**\*</span><span class="sxs-lookup"><span data-stu-id="3876e-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="3876e-109">Reveja a descrição para ver as condições configuradas que afetaram a mensagem.</span><span class="sxs-lookup"><span data-stu-id="3876e-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="3876e-110">Para saber mais, consulte [a Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="3876e-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
