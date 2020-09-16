---
title: Limite diário de e-mail excedido. O fluxo de trabalho está suspenso.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731574"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limite de e-mail diário ultrapassado. O fluxo de trabalho está suspenso.

Este erro pode ser recebido nos seguintes cenários:

- Tem um fluxo de trabalho no SharePoint Online que está a utilizar o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.
- O fluxo de trabalho está configurado para enviar uma mensagem de correio eletrónico personalizada a mais de 200 utilizadores de cada vez, mais de 10.000 destinatários por dia, ou mais de 30 mensagens por minuto.
- Quando executam o fluxo de trabalho, a mensagem de e-mail não é enviada e nota o seguinte comportamento:
    - Para um fluxo de trabalho utilizando o tipo de plataforma SharePoint 2013, navegue na página **'Estado do Fluxo de Trabalho'.** Na página 'Estado do Fluxo de Trabalho', o **Estado Interno** está definido para **Iniciar**, e o balão de informação **apresenta-se Incapaz de enviar para um destinatário**.

Para contornar este problema, configuure o seu fluxo de trabalho para enviar mensagens de correio eletrónico sem exceder os [limites de remetente Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Por exemplo, use uma pausa no fluxo de trabalho, envie o e-mail para um grupo Microsoft 365, um grupo de distribuição ou grupo de segurança habilitado por correio, ou envie a mensagem para menos de 200 destinatários de cada vez.


Para mais informações, consulte o seguinte [artigo.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Tópicos relacionados
- [Criar Fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 