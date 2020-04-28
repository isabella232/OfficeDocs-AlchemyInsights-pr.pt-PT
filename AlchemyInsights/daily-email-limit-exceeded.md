---
title: Limite diário de e-mail ultrapassado. O fluxo de trabalho está suspenso.
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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908715"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="15885-103">Limite de e-mail diário ultrapassado.</span><span class="sxs-lookup"><span data-stu-id="15885-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="15885-104">O fluxo de trabalho está suspenso.</span><span class="sxs-lookup"><span data-stu-id="15885-104">Workflow is suspended.</span></span>

<span data-ttu-id="15885-105">Este erro pode ser recebido nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="15885-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="15885-106">Tem um fluxo de trabalho no SharePoint Online que está a usar o tipo de plataforma de fluxo de trabalho SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="15885-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="15885-107">O fluxo de trabalho está configurado para enviar uma mensagem de correio eletrónico personalizada a mais de 200 utilizadores de cada vez, mais de 10.000 destinatários por dia, ou mais de 30 mensagens por minuto.</span><span class="sxs-lookup"><span data-stu-id="15885-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="15885-108">Quando executa o fluxo de trabalho, a mensagem de e-mail não é enviada, e você nota o seguinte comportamento:</span><span class="sxs-lookup"><span data-stu-id="15885-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="15885-109">Para um fluxo de trabalho utilizando o tipo de plataforma SharePoint 2013, você navega para a página **Workflow Status.**</span><span class="sxs-lookup"><span data-stu-id="15885-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="15885-110">Na página do Estado do Fluxo de Trabalho, o **Estado Interno** está definido para **Iniciar**, e o balão de informação mostra Incapaz de enviar a **um destinatário**.</span><span class="sxs-lookup"><span data-stu-id="15885-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="15885-111">Para resolver este problema, configure o seu fluxo de trabalho para enviar mensagens de correio eletrónico sem exceder os limites de [remetente exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="15885-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="15885-112">Por exemplo, utilize uma pausa no fluxo de trabalho, envie o e-mail para um grupo Microsoft 365, um grupo de distribuição ou grupo de segurança ativado por correio, ou envie a mensagem para menos de 200 destinatários de cada vez.</span><span class="sxs-lookup"><span data-stu-id="15885-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="15885-113">Para mais informações, consulte o [seguinte artigo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="15885-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="15885-114">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="15885-114">Related topics</span></span>
- [<span data-ttu-id="15885-115">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="15885-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="15885-116">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="15885-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 