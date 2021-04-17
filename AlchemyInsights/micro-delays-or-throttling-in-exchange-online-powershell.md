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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro atrasos ou limitação no PowerShell do Exchange Online

Poderá ver avisos ou atrasos com a mensagem "Micro atraso aplicado" ao executar scripts ou cmdlets no Exchange Online, Seguem-se duas sugestões relacionadas com este problema:

- É aconselhável tentar utilizar o [módulo Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), que inclui CMDlets baseados em REST API, com um desempenho significativamente superior. Esta pode ser uma ótima solução para muitos Get- CMDlets que são frequentemente usados.
- Se precisar de utilizar CMDlets que ainda não estejam cobertos pelo módulo v2, consulte [Executar cmdlets do PowerShell para grandes números de utilizadores no Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que aborda a forma de contornar os limites esperados do PowerShell no Exchange Online.
