---
title: mesmo que o nome de ficheiro é o melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676544"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="97f10-102">Exigia alquimia cabeçalho H1, H2's não funciona.</span><span class="sxs-lookup"><span data-stu-id="97f10-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="97f10-103">Boas Práticas e orientações para a autoria da Alquimia:</span><span class="sxs-lookup"><span data-stu-id="97f10-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="97f10-104">**Não nidique alquimia insights em pastas**- isto quebrará a estrutura do url.</span><span class="sxs-lookup"><span data-stu-id="97f10-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="97f10-105">Estamos a tentar resolver isto.</span><span class="sxs-lookup"><span data-stu-id="97f10-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="97f10-106">Os ficheiros na pasta **AlchemyInsights** devem ter nomes de ficheiros minúsculos com hífens para espaços ex.</span><span class="sxs-lookup"><span data-stu-id="97f10-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="97f10-107">***como permitir-ativar-contencioso-hold***.</span><span class="sxs-lookup"><span data-stu-id="97f10-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="97f10-108">Inclua o ID de regra ou id balde do [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) no campo ms.custom.</span><span class="sxs-lookup"><span data-stu-id="97f10-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="97f10-109">ex.</span><span class="sxs-lookup"><span data-stu-id="97f10-109">ex.</span></span> <span data-ttu-id="97f10-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="97f10-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="97f10-111">Utilize o resto dos metadados na parte superior deste ficheiro como modelo.</span><span class="sxs-lookup"><span data-stu-id="97f10-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="97f10-112">No [portal Alchemy Partner,](https://alchemyportal.azurewebsites.net)navegue até à secção Título de Insight do **Cliente:** e use-o como ponto de partida para o seu título de H1 para a insight.</span><span class="sxs-lookup"><span data-stu-id="97f10-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="97f10-113">Alquimia Insights MUST tem apenas um único H1 no topo ou eles vão quebrar na produção.</span><span class="sxs-lookup"><span data-stu-id="97f10-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="97f10-114">Os H2 não prestam nem por isso use convenções **ousadas** ou outras para significar secções separadas.</span><span class="sxs-lookup"><span data-stu-id="97f10-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="97f10-115">Em seguida, preencha o texto do corpo utilizando o projeto de material na secção Deinsights do Cliente da página regra da Alquimia</span><span class="sxs-lookup"><span data-stu-id="97f10-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="97f10-116">Listas de balas estão bem.</span><span class="sxs-lookup"><span data-stu-id="97f10-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="97f10-117">Listas numeradas também</span><span class="sxs-lookup"><span data-stu-id="97f10-117">Numbered lists too</span></span>
    1. <span data-ttu-id="97f10-118">**Arrojado** e *itálico* são um ok</span><span class="sxs-lookup"><span data-stu-id="97f10-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="97f10-119">As ligações devem ser sempre **"links para web"/external** OU **deep-links para elementos UI**, e não ligações internas.</span><span class="sxs-lookup"><span data-stu-id="97f10-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="97f10-120">As imagens não são oficialmente apoiadas neste momento, mas está no roteiro.</span><span class="sxs-lookup"><span data-stu-id="97f10-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="97f10-121">E isto já é um pouco longo demais.</span><span class="sxs-lookup"><span data-stu-id="97f10-121">And this is really already a bit too long.</span></span> <span data-ttu-id="97f10-122">A melhor prática é cerca de 400 caracteres ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="97f10-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="97f10-123">Assim que o conteúdo estiver pronto, puxe-o para o ramo vivo.</span><span class="sxs-lookup"><span data-stu-id="97f10-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="97f10-124">Em seguida, vá ao [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) e introduza o nome de ficheiro no campo de url.</span><span class="sxs-lookup"><span data-stu-id="97f10-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 