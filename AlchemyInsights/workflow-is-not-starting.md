---
title: Fluxo de trabalho não está iniciando
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738100"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="e0449-102">Fluxo de trabalho não está iniciando</span><span class="sxs-lookup"><span data-stu-id="e0449-102">Workflow is not starting</span></span>

- <span data-ttu-id="e0449-103">Fluxos de trabalho do SharePoint 2010 e SharePoint 2013 não estão iniciando.</span><span class="sxs-lookup"><span data-stu-id="e0449-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="e0449-104">Se o fluxo de trabalho não estiver iniciando, pode haver um problema de serviço temporário em que os usuários podem enfrentar atrasos intermitentes com o andamento do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0449-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="e0449-105">Verifique o [painel de integridade do serviço](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização foi afetada.</span><span class="sxs-lookup"><span data-stu-id="e0449-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="e0449-106">Se mais de 24 horas se passaram desde que você viu este problema pela primeira vez, por favor, registre um ticket de suporte.</span><span class="sxs-lookup"><span data-stu-id="e0449-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="e0449-107">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="e0449-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e0449-108">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="e0449-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="e0449-109">Fluxos de trabalho do SharePoint 2010 atrasados no início.</span><span class="sxs-lookup"><span data-stu-id="e0449-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="e0449-110">Isso ocorre se o fluxo de trabalho é acionado em lotes grandes.</span><span class="sxs-lookup"><span data-stu-id="e0449-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="e0449-111">(por exemplo, quando vários itens são adicionados de uma só vez).</span><span class="sxs-lookup"><span data-stu-id="e0449-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="e0449-112">Fluxos de trabalho não são projetados para executar em tempo real, portanto, um atraso é o comportamento de design.</span><span class="sxs-lookup"><span data-stu-id="e0449-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="e0449-113">Se o fluxo de trabalho é complexo Extensible Object Markup Language (XMOL), compilação pode ser lenta.</span><span class="sxs-lookup"><span data-stu-id="e0449-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="e0449-114">Verifique [este](https://support.microsoft.com//kb/3043697) artigo.</span><span class="sxs-lookup"><span data-stu-id="e0449-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="e0449-115">Você deve simplificar o fluxo de trabalho ou reformulá-lo usando o tipo de plataforma Microsoft SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="e0449-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="e0449-116">Se o histórico de fluxo de trabalho cresceu grande, convém limpar os itens ou criar uma nova lista de histórico.</span><span class="sxs-lookup"><span data-stu-id="e0449-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="e0449-117">Mais informações: [Limpar histórico de fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="e0449-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="e0449-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="e0449-118">Related topics</span></span>
<span data-ttu-id="e0449-119">Deseja experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e0449-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e0449-120">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="e0449-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e0449-121">SharePoint e fluxo</span><span class="sxs-lookup"><span data-stu-id="e0449-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


