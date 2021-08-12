---
title: O limite diário de e-mails foi excedido. O fluxo de trabalho está suspenso.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914662"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite diário de e-mail Excedido. O fluxo de trabalho está suspenso.

Este erro pode ser recebido nos seguintes cenários:

- Tem um fluxo de trabalho no SharePoint Online que utiliza o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.
- O fluxo de trabalho está configurado para enviar uma mensagem de e-mail personalizada a mais de 200 utilizadores de cada vez, mais de 10 000 destinatários por dia ou mais de 30 mensagens por minuto.
- Quando executa o fluxo de trabalho, a mensagem de e-mail não é enviada e nota o seguinte comportamento:
    - Para um fluxo de trabalho com o tipo de plataforma SharePoint 2013, navegue até à **página Estado do Fluxo de** Trabalho. Na página Estado do Fluxo de Trabalho, o Estado **Interno** está definido como Iniciado e o balão de informações é apresentado como Não é possível **enviar para um destinatário.** 

Para resolver este problema, configure o seu fluxo de trabalho para enviar mensagens de e-mail sem exceder os [limites Exchange Online remetente da mensagem](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Por exemplo, utilize uma pausa no fluxo de trabalho, envie o e-mail para um grupo do Microsoft 365, para um grupo de distribuição ou para um grupo de segurança com capacidade de correio ou envie a mensagem para menos de 200 destinatários de cada vez.


Para obter mais informações, consulte o seguinte [artigo.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Tópicos relacionados
- [Criar Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 