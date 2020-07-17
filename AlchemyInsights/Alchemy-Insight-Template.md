---
title: mesmo que nome de arquivo é melhor
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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750981"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="8f692-102">"Cabeçalho de Alquimia H1, H2 não funciona."</span><span class="sxs-lookup"><span data-stu-id="8f692-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="8f692-103">Boas Práticas e orientações para a autoria da Alquimia:</span><span class="sxs-lookup"><span data-stu-id="8f692-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="8f692-104">**Não aninhar a Alquimia Insights em pastas**- isto quebrará a estrutura url.</span><span class="sxs-lookup"><span data-stu-id="8f692-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="8f692-105">Estamos a tentar resolver isto.</span><span class="sxs-lookup"><span data-stu-id="8f692-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="8f692-106">Os ficheiros na pasta **AlchemyInsights** devem ter canções minúsculas com hífenes para espaços ex.</span><span class="sxs-lookup"><span data-stu-id="8f692-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="8f692-107">***como permitir-permitir litígios- hold***.</span><span class="sxs-lookup"><span data-stu-id="8f692-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="8f692-108">Inclua o ID de Regra ou ID do balde do [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) no campo ms.custom.</span><span class="sxs-lookup"><span data-stu-id="8f692-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="8f692-109">ex.</span><span class="sxs-lookup"><span data-stu-id="8f692-109">ex.</span></span> <span data-ttu-id="8f692-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="8f692-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="8f692-111">Utilize o resto dos metadados na parte superior deste ficheiro como modelo.</span><span class="sxs-lookup"><span data-stu-id="8f692-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="8f692-112">No [portal Alchemy Partner,](https://alchemyportal.azurewebsites.net)navegue até à secção **Título de Insight do Cliente:** e use-o como ponto de partida para o seu título H1 para a visão.</span><span class="sxs-lookup"><span data-stu-id="8f692-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="8f692-113">A Alquimia Insights DEVE ter apenas um H1 no topo ou eles vão quebrar a produção.</span><span class="sxs-lookup"><span data-stu-id="8f692-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="8f692-114">Os H2 não prestam nem por isso usam convenções **ousadas** ou outras para significar secções separadas.</span><span class="sxs-lookup"><span data-stu-id="8f692-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="8f692-115">Em seguida, preencha o texto do corpo utilizando o material de projeto na secção de Insights do Cliente da página Regra da Alquimia</span><span class="sxs-lookup"><span data-stu-id="8f692-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="8f692-116">As listas de balas estão bem.</span><span class="sxs-lookup"><span data-stu-id="8f692-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="8f692-117">Listas numeradas também</span><span class="sxs-lookup"><span data-stu-id="8f692-117">Numbered lists too</span></span>
    1. <span data-ttu-id="8f692-118">**Arrojado** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="8f692-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="8f692-119">As ligações devem ser sempre **"links para web"/external** OU **ligações profundas a elementos de UI,** e não ligações internas.</span><span class="sxs-lookup"><span data-stu-id="8f692-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="8f692-120">As fotos não são oficialmente suportadas neste momento, mas está no roteiro.</span><span class="sxs-lookup"><span data-stu-id="8f692-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="8f692-121">E isto já é um pouco longo demais.</span><span class="sxs-lookup"><span data-stu-id="8f692-121">And this is really already a bit too long.</span></span> <span data-ttu-id="8f692-122">A melhor prática é cerca de 400 caracteres ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="8f692-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="8f692-123">Assim que o seu conteúdo estiver pronto, puxe-o para o ramo ao vivo.</span><span class="sxs-lookup"><span data-stu-id="8f692-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="8f692-124">Em seguida, vá ao [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) e introduza o nome de arquivo no campo url.</span><span class="sxs-lookup"><span data-stu-id="8f692-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 