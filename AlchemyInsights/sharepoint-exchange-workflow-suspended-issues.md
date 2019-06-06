---
title: Começar a trabalhar com SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: a44b2c7b26895e09c24df772f1ada9a2e3483747
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735993"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="2eb7f-102">Fluxos de trabalho no SharePoint</span><span class="sxs-lookup"><span data-stu-id="2eb7f-102">Workflows in SharePoint</span></span>

<span data-ttu-id="2eb7f-103">Se os fluxos de trabalho do SharePoint não estão a enviar mensagens de correio electrónico, a organização poderá ter encontrado os limites de remetente Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2eb7f-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="2eb7f-104">'Fluxo de trabalho é suspenso' mensagem de erro poderá ocorrer se tiver um dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="2eb7f-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="2eb7f-105">Ter um fluxo de trabalho no SharePoint Online que está a utilizar o SharePoint 2010 ou o tipo de plataforma de fluxo de trabalho do SharePoint de 2013.</span><span class="sxs-lookup"><span data-stu-id="2eb7f-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="2eb7f-106">O fluxo de trabalho está configurado para enviar uma mensagem de correio electrónico personalizado a mais de 200 utilizadores cada vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="2eb7f-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="2eb7f-107">Quando executar o fluxo de trabalho, a mensagem de correio electrónico não é enviada e repare a mensagem de erro, o estado interno estiver definido como suspenso ou não é possível enviar para um destinatário é apresentado.</span><span class="sxs-lookup"><span data-stu-id="2eb7f-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="2eb7f-108">Para mais informações, consulte o seguinte [artigo](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="2eb7f-108">For more information, please refer to the following [article](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

