---
title: O fluxo de trabalho não está a começar
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403754"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="a59c9-102">O fluxo de trabalho não está a começar</span><span class="sxs-lookup"><span data-stu-id="a59c9-102">Workflow is not starting</span></span>

- <span data-ttu-id="a59c9-103">Os fluxos de trabalho do SharePoint 2010 e do SharePoint 2013 não estão a começar.</span><span class="sxs-lookup"><span data-stu-id="a59c9-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="a59c9-104">Se o seu fluxo de trabalho não estiver a começar, pode haver um problema de serviço temporário onde os utilizadores podem sofrer atrasos intermitentes com o progresso do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a59c9-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="a59c9-105">Consulte o [Painel de Saúde](https://admin.microsoft.com/AdminPortal/Home/servicehealth) do Serviço para ver se a sua organização está com impacto.</span><span class="sxs-lookup"><span data-stu-id="a59c9-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="a59c9-106">Se passaram mais de 24 horas desde que viu este problema pela primeira vez, por favor, faça um bilhete de apoio.</span><span class="sxs-lookup"><span data-stu-id="a59c9-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a59c9-107">Em muitos casos, já estamos a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="a59c9-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a59c9-108">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="a59c9-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="a59c9-109">Fluxos de trabalho sharePoint 2010 adiados no início.</span><span class="sxs-lookup"><span data-stu-id="a59c9-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="a59c9-110">Isto ocorre se o fluxo de trabalho for acionado em grandes lotes.</span><span class="sxs-lookup"><span data-stu-id="a59c9-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="a59c9-111">(por exemplo, quando vários itens são adicionados ao mesmo tempo).</span><span class="sxs-lookup"><span data-stu-id="a59c9-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="a59c9-112">Os fluxos de trabalho não são projetados para funcionar em tempo real, por isso um atraso é o comportamento por design.</span><span class="sxs-lookup"><span data-stu-id="a59c9-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="a59c9-113">Se o fluxo de trabalho for complexo lingueta de marcação de objetos extensíveis (XMOL), a compilação pode ser lenta.</span><span class="sxs-lookup"><span data-stu-id="a59c9-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="a59c9-114">Veja [este](https://support.microsoft.com//kb/3043697) artigo.</span><span class="sxs-lookup"><span data-stu-id="a59c9-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="a59c9-115">Deve simplificar o fluxo de trabalho ou redesenhar-o utilizando o tipo de plataforma de fluxo de trabalho Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="a59c9-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="a59c9-116">Se o seu histórico de fluxo de trabalho cresceu, pode querer purgar os itens ou criar uma nova lista de histórias.</span><span class="sxs-lookup"><span data-stu-id="a59c9-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="a59c9-117">Mais informações : [Purgar a história do fluxo de trabalho](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="a59c9-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="a59c9-118">Tópicos relacionados</span><span class="sxs-lookup"><span data-stu-id="a59c9-118">Related topics</span></span>
<span data-ttu-id="a59c9-119">Quer experimentar o Microsoft Flow no SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a59c9-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a59c9-120">Criar Fluxo</span><span class="sxs-lookup"><span data-stu-id="a59c9-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a59c9-121">SharePoint e Flow</span><span class="sxs-lookup"><span data-stu-id="a59c9-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
