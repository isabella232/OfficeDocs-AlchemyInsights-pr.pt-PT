---
title: Comece com sharepoint on-line
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051652"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="dc500-102">Fluxos de trabalho no SharePoint</span><span class="sxs-lookup"><span data-stu-id="dc500-102">Workflows in SharePoint</span></span>

<span data-ttu-id="dc500-103">Se os fluxos de trabalho do SharePoint não estiverem enviando e-mails, sua organização poderá ter encontrado os limites do remetente da Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="dc500-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="dc500-104">A mensagem de erro "Fluxo de trabalho está suspenso" pode ocorrer se você tiver um dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="dc500-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="dc500-105">Você tem um fluxo de trabalho no SharePoint Online que está usando o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="dc500-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="dc500-106">O fluxo de trabalho está configurado para enviar uma mensagem de e-mail personalizada para mais de 200 usuários de cada vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="dc500-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="dc500-107">Quando você executar o fluxo de trabalho, a mensagem de e-mail não é enviada e você percebe a mensagem de erro, o status interno é definido para suspenso ou incapaz de enviar para um destinatário é exibido.</span><span class="sxs-lookup"><span data-stu-id="dc500-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="dc500-108">Para mais informações, consulte o seguinte [artigo.](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)</span><span class="sxs-lookup"><span data-stu-id="dc500-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

