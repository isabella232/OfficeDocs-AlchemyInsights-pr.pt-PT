---
title: Micro atrasos ou limitação no PowerShell do Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702137"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="bc78e-102">Micro atrasos ou limitação no PowerShell do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="bc78e-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="bc78e-103">Poderá ver avisos ou atrasos com a mensagem "Micro atraso aplicado" ao executar scripts ou cmdlets no Exchange Online,</span><span class="sxs-lookup"><span data-stu-id="bc78e-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="bc78e-104">Eis algumas sugestões sobre como resolver este problema:</span><span class="sxs-lookup"><span data-stu-id="bc78e-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="bc78e-105">Execute os nossos diagnósticos para descontrair as políticas de throttling do PowerShell do seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="bc78e-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="bc78e-106">Esta solução irá resolver o problema para a maioria dos problemas.</span><span class="sxs-lookup"><span data-stu-id="bc78e-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="bc78e-107">Se o problema continuar a não ser resolvido, utilize [o módulo Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), que inclui cmdlets baseados na API REST e que têm um melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="bc78e-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="bc78e-108">Esta pode ser uma ótima solução para muitos Get- CMDlets que são frequentemente usados.</span><span class="sxs-lookup"><span data-stu-id="bc78e-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="bc78e-109">Se precisar de utilizar CMDlets que não são abrangidos pelo módulo v2, consulte Executar [cmdlets do PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)para um grande número de utilizadores no Office 365, que fala sobre como utilizar limites de limitação do PowerShell no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="bc78e-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
