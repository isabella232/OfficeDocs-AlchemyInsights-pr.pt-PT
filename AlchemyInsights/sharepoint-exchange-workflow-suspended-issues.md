---
title: Começar a trabalhar com SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751683"
---
# <a name="workflows-in-sharepoint"></a>Fluxos de trabalho no SharePoint

Se os fluxos de trabalho do SharePoint não estão a enviar mensagens de correio electrónico, a organização poderá ter encontrado os limites de remetente Exchange Online.

'Fluxo de trabalho é suspenso' mensagem de erro poderá ocorrer se tiver um dos seguintes itens:

- Ter um fluxo de trabalho no SharePoint Online que está a utilizar o SharePoint 2010 ou o tipo de plataforma de fluxo de trabalho do SharePoint de 2013.

- O fluxo de trabalho está configurado para enviar uma mensagem de correio electrónico personalizado a mais de 200 utilizadores cada vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.

Quando executar o fluxo de trabalho, a mensagem de correio electrónico não é enviada e repare a mensagem de erro, o estado interno estiver definido como suspenso ou não é possível enviar para um destinatário é apresentado.

Para mais informações, consulte o seguinte [artigo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

