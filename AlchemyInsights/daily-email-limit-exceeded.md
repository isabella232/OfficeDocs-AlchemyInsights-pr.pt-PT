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
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="6d7f6-103">Correio electrónico diário limite excedido.</span><span class="sxs-lookup"><span data-stu-id="6d7f6-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="6d7f6-104">Fluxo de trabalho é suspenso.</span><span class="sxs-lookup"><span data-stu-id="6d7f6-104">Workflow is suspended.</span></span>

<span data-ttu-id="6d7f6-105">Este erro pode ser recebido nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="6d7f6-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="6d7f6-106">Ter um fluxo de trabalho no SharePoint Online que está a utilizar o SharePoint 2010 ou o tipo de plataforma de fluxo de trabalho do SharePoint de 2013.</span><span class="sxs-lookup"><span data-stu-id="6d7f6-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="6d7f6-107">O fluxo de trabalho está configurado para enviar uma mensagem de correio electrónico personalizado a mais de 200 utilizadores cada vez, mais de 10.000 destinatários por dia ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="6d7f6-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="6d7f6-108">Quando executar o fluxo de trabalho, a mensagem de correio electrónico não é enviada e detectar o seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="6d7f6-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="6d7f6-109">Para um fluxo de trabalho utilizando o tipo de plataforma do SharePoint de 2013, navegue para a página **Estado do fluxo de trabalho** .</span><span class="sxs-lookup"><span data-stu-id="6d7f6-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="6d7f6-110">Na página Estado do fluxo de trabalho, o **Estado interno** está definido como **iniciado**e o balão de informações apresenta **não foi possível enviar para um destinatário**.</span><span class="sxs-lookup"><span data-stu-id="6d7f6-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="6d7f6-111">Para contornar este problema, configure o fluxo de trabalho para enviar mensagens de correio electrónico sem exceder os [limites de remetente Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="6d7f6-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="6d7f6-112">Por exemplo, utilize uma pausa no fluxo de trabalho, enviar mensagem de correio electrónico para um grupo do Office 365, um grupo de distribuição ou grupo de segurança de capacidade para correio electrónico ou enviar a mensagem para menos de 200 destinatários ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6d7f6-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="6d7f6-113">Para mais informações, consulte o seguinte [artigo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="6d7f6-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="6d7f6-114">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="6d7f6-114">Related topics</span></span>
- [<span data-ttu-id="6d7f6-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="6d7f6-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6d7f6-116">Fluxo e do SharePoint</span><span class="sxs-lookup"><span data-stu-id="6d7f6-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 