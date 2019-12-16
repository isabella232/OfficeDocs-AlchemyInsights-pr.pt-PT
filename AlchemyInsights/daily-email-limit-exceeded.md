---
title: Limite de e-mail diário ultrapassado. O fluxo de trabalho está suspenso.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053128"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite de e-mail diário ultrapassado. O fluxo de trabalho está suspenso.

Esse erro pode ser recebido nos seguintes cenários:

- Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.
- O fluxo de trabalho está configurado para enviar uma mensagem de e-mail personalizada para mais de 200 usuários de cada vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.
- Quando você executar o fluxo de trabalho, a mensagem de e-mail não é enviada, e você percebe o seguinte comportamento:
    - Para um fluxo de trabalho usando o tipo de plataforma SharePoint 2013, você navega na página de status do fluxo de **trabalho.** Na página de status do fluxo de trabalho, o **status interno** está definido para **iniciado,** e o balão de informações exibe **incapaz de enviar a um destinatário.**

Para contornar esse problema, configure seu fluxo de trabalho para enviar mensagens de e-mail sem exceder os limites do [remetente da Exchange Online.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Por exemplo, use uma pausa no fluxo de trabalho, envie o e-mail para um grupo do Office 365, um grupo de distribuição ou um grupo de segurança habilitado por e-mail ou envie a mensagem para menos de 200 destinatários de cada vez.


Para mais informações, consulte o seguinte [artigo.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Tópicos relacionados
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 