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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868545"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro atrasos ou limitação no PowerShell do Exchange Online

Poderá ver avisos ou atrasos com a mensagem "Micro atraso aplicado" ao executar scripts ou cmdlets no Exchange Online, Eis algumas sugestões sobre como resolver este problema:

- Execute os nossos diagnósticos para descontrair as políticas de throttling do PowerShell do seu inquilino. Esta solução irá resolver o problema para a maioria dos problemas.
- Se o problema continuar a não ser resolvido, utilize [o módulo Exchange Online v2 powerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), que inclui cmdlets baseados na API REST e que têm um melhor desempenho. Esta pode ser uma ótima solução para muitos Get- CMDlets que são frequentemente usados.
- Se precisar de utilizar CMDlets que não são abrangidos pelo módulo v2, consulte Executar [cmdlets do PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)para um grande número de utilizadores no Office 365, que fala sobre como utilizar limites de limitação do PowerShell no Exchange Online.
