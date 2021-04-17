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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830044"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="a0be3-102">Micro atrasos ou limitação no PowerShell do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a0be3-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="a0be3-103">Poderá ver avisos ou atrasos com a mensagem "Micro atraso aplicado" ao executar scripts ou cmdlets no Exchange Online,</span><span class="sxs-lookup"><span data-stu-id="a0be3-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="a0be3-104">Seguem-se duas sugestões relacionadas com este problema:</span><span class="sxs-lookup"><span data-stu-id="a0be3-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="a0be3-105">É aconselhável tentar utilizar o [módulo Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), que inclui CMDlets baseados em REST API, com um desempenho significativamente superior.</span><span class="sxs-lookup"><span data-stu-id="a0be3-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="a0be3-106">Esta pode ser uma ótima solução para muitos Get- CMDlets que são frequentemente usados.</span><span class="sxs-lookup"><span data-stu-id="a0be3-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="a0be3-107">Se precisar de utilizar CMDlets que ainda não estejam cobertos pelo módulo v2, consulte [Executar cmdlets do PowerShell para grandes números de utilizadores no Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que aborda a forma de contornar os limites esperados do PowerShell no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a0be3-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
