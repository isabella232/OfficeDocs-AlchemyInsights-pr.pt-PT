---
title: O fluxo de trabalho não está a começar
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049348"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="942d0-102">O fluxo de trabalho não está a começar</span><span class="sxs-lookup"><span data-stu-id="942d0-102">Workflow is not starting</span></span>

- <span data-ttu-id="942d0-103">Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão começando.</span><span class="sxs-lookup"><span data-stu-id="942d0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="942d0-104">Se o seu fluxo de trabalho não estiver a começar, poderá haver um problema de serviço temporário em que os utilizadores podem sofrer atrasos intermitentes com o progresso do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="942d0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="942d0-105">Verifique o Painel de Saúde do [Serviço](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização está afetada.</span><span class="sxs-lookup"><span data-stu-id="942d0-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="942d0-106">Se mais de 24 horas se passaram desde que você viu pela primeira vez este problema, por favor, registre um bilhete de suporte.</span><span class="sxs-lookup"><span data-stu-id="942d0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="942d0-107">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="942d0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="942d0-108">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="942d0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="942d0-109">Os fluxos de trabalho do SharePoint 2010 atrasaram no início.</span><span class="sxs-lookup"><span data-stu-id="942d0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="942d0-110">Isso ocorre se o fluxo de trabalho for acionado em grandes lotes.</span><span class="sxs-lookup"><span data-stu-id="942d0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="942d0-111">(por exemplo, quando vários itens são adicionados ao mesmo tempo).</span><span class="sxs-lookup"><span data-stu-id="942d0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="942d0-112">Os fluxos de trabalho não são projetados para serem executados em tempo real, então um atraso é o comportamento de design por ação.</span><span class="sxs-lookup"><span data-stu-id="942d0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="942d0-113">Se o fluxo de trabalho for complexo da Linguagem de Marcação de Objetoextensível (XMOL), a compilação pode ser lenta.</span><span class="sxs-lookup"><span data-stu-id="942d0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="942d0-114">Confira [este](https://support.microsoft.com//kb/3043697) artigo.</span><span class="sxs-lookup"><span data-stu-id="942d0-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="942d0-115">Você deve simplificar o fluxo de trabalho ou reprojetá-lo usando o tipo de plataforma de fluxo de trabalho Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="942d0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="942d0-116">Se o seu histórico de fluxo de trabalho cresceu, você pode querer limpar os itens ou criar uma nova lista de história.</span><span class="sxs-lookup"><span data-stu-id="942d0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="942d0-117">Mais informações: [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="942d0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="942d0-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="942d0-118">Related topics</span></span>
<span data-ttu-id="942d0-119">Quer experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="942d0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="942d0-120">Criar fluxo</span><span class="sxs-lookup"><span data-stu-id="942d0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="942d0-121">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="942d0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


