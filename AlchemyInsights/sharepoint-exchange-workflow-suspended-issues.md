---
title: Começar a trabalhar com o SharePoint Online
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
ms.openlocfilehash: a14705003f742641f10c8459b7c7024146e4134a8d5113451e5732cef7326484
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54051425"
---
# <a name="workflows-in-sharepoint"></a>Fluxos de trabalho no SharePoint

Se os fluxos de trabalho do SharePoint não estiverem a enviar e-mails, a sua organização poderá ter encontrado os limites Exchange Online remetente da mensagem.

A mensagem de erro "Fluxo de Trabalho está Suspenso" pode ocorrer se tiver um dos seguintes itens:

- Tem um fluxo de trabalho no SharePoint Online que utiliza o tipo de plataforma de fluxo de trabalho do SharePoint 2010 ou SharePoint 2013.

- O fluxo de trabalho está configurado para enviar uma mensagem de e-mail personalizada a mais de 200 utilizadores de cada vez, mais de 10 000 destinatários por dia ou mais de 30 mensagens por minuto.

Quando executa o fluxo de trabalho, a mensagem de e-mail não é enviada e nota a mensagem de erro, o Estado Interno está definido como Suspenso ou Não é possível enviar para um destinatário é apresentado.

Para obter mais informações, consulte o seguinte [artigo.](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)

