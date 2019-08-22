---
title: Limite de correio electrónico diária foi excedido. Fluxo de trabalho é suspenso.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514477"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Correio electrónico diário limite excedido. Fluxo de trabalho é suspenso.

Este erro pode ser recebido nos seguintes cenários:

- Ter um fluxo de trabalho no SharePoint Online que está a utilizar o SharePoint 2010 ou o tipo de plataforma de fluxo de trabalho do SharePoint de 2013.
- O fluxo de trabalho está configurado para enviar uma mensagem de correio electrónico personalizado a mais de 200 utilizadores cada vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.
- Quando executar o fluxo de trabalho, a mensagem de correio electrónico não é enviada e detectar o seguinte comportamento:
    - Para um fluxo de trabalho utilizando o tipo de plataforma do SharePoint de 2013, navegue para a página **Estado do fluxo de trabalho** . Na página Estado do fluxo de trabalho, o **Estado interno** está definido como **iniciado**e o balão de informações apresenta **não foi possível enviar para um destinatário**.

Para contornar este problema, configure o fluxo de trabalho para enviar mensagens de correio electrónico sem exceder os [limites de remetente Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Por exemplo, utilize uma pausa no fluxo de trabalho, enviar mensagem de correio electrónico para um grupo do Office 365, um grupo de distribuição ou grupo de segurança de capacidade para correio electrónico ou enviar a mensagem para menos de 200 destinatários ao mesmo tempo.


Para mais informações, consulte o seguinte [artigo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Tópicos relacionados
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Fluxo e do SharePoint](https://flow.microsoft.com/blog/sharepoint-and-flow/) 