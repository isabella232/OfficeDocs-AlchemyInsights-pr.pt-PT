---
title: Começar com o SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700718"
---
# <a name="workflows-in-sharepoint"></a>Fluxos de trabalho no SharePoint

Se os fluxos de trabalho do SharePoint não estiverem a enviar e-mails, a sua organização pode ter encontrado os limites do remetente Exchange Online.

A mensagem de erro 'Workflow is Suspended' pode ocorrer se tiver um dos seguintes itens:

- Tem um fluxo de trabalho no SharePoint Online que está a utilizar o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.

- O fluxo de trabalho está configurado para enviar uma mensagem de correio eletrónico personalizada a mais de 200 utilizadores de cada vez, mais de 10.000 destinatários por dia, ou mais de 30 mensagens por minuto.

Quando executam o fluxo de trabalho, a mensagem de correio eletrónico não é enviada e nota a mensagem de erro, o Estado Interno está definido para Suspenso ou Não é possível enviar para um destinatário.

Para mais informações, consulte o [seguinte artigo.](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)

