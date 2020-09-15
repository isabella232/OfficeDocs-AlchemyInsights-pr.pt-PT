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
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="1e9ed-102">Fluxos de trabalho no SharePoint</span><span class="sxs-lookup"><span data-stu-id="1e9ed-102">Workflows in SharePoint</span></span>

<span data-ttu-id="1e9ed-103">Se os fluxos de trabalho do SharePoint não estiverem a enviar e-mails, a sua organização pode ter encontrado os limites do remetente Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1e9ed-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="1e9ed-104">A mensagem de erro 'Workflow is Suspended' pode ocorrer se tiver um dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="1e9ed-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="1e9ed-105">Tem um fluxo de trabalho no SharePoint Online que está a utilizar o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="1e9ed-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="1e9ed-106">O fluxo de trabalho está configurado para enviar uma mensagem de correio eletrónico personalizada a mais de 200 utilizadores de cada vez, mais de 10.000 destinatários por dia, ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="1e9ed-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="1e9ed-107">Quando executam o fluxo de trabalho, a mensagem de correio eletrónico não é enviada e nota a mensagem de erro, o Estado Interno está definido para Suspenso ou Não é possível enviar para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="1e9ed-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="1e9ed-108">Para mais informações, consulte o [seguinte artigo.](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)</span><span class="sxs-lookup"><span data-stu-id="1e9ed-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

