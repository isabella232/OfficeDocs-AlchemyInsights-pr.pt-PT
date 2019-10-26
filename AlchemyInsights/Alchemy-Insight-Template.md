---
title: mesmo que o nome de arquivo é melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800056"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="190bb-102">Obrigado Alquimia Cabeçalho H1, H2 não funcionam.</span><span class="sxs-lookup"><span data-stu-id="190bb-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="190bb-103">Melhores práticas e diretrizes para a autoria da Alquimia:</span><span class="sxs-lookup"><span data-stu-id="190bb-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="190bb-104">**Não aninhe Alchemy Insights em pastas**- isso vai quebrar a estrutura url.</span><span class="sxs-lookup"><span data-stu-id="190bb-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="190bb-105">Estamos procurando consertar isso.</span><span class="sxs-lookup"><span data-stu-id="190bb-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="190bb-106">Arquivos na pasta **AlchemyInsights** devem ter nomes de arquivos minúsculos com hífens para espaços ex.</span><span class="sxs-lookup"><span data-stu-id="190bb-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="190bb-107">***como habilitar-litígio-hold***.</span><span class="sxs-lookup"><span data-stu-id="190bb-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="190bb-108">Inclua a identificação da régua ou a identificação do balde do portal do sócio da [alquimia](https://alchemyportal.azurewebsites.net) no campo do ms.custom.</span><span class="sxs-lookup"><span data-stu-id="190bb-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="190bb-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="190bb-109">ex.</span></span> <span data-ttu-id="190bb-110">***ms.custom: 100021 ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="190bb-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="190bb-111">Use o resto dos metadados na parte superior deste arquivo como modelo.</span><span class="sxs-lookup"><span data-stu-id="190bb-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="190bb-112">No [portal Alchemy Partner,](https://alchemyportal.azurewebsites.net)navegue até a seção Título de Percepção do **Cliente:** e use isso como ponto de partida para o seu título H1 para obter informações.</span><span class="sxs-lookup"><span data-stu-id="190bb-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="190bb-113">Alquimia Insights deve ter apenas um único H1 no topo ou eles vão quebrar na produção.</span><span class="sxs-lookup"><span data-stu-id="190bb-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="190bb-114">Os H2s não tornam o **uso ousado** ou outras convenções para significar seções separadas.</span><span class="sxs-lookup"><span data-stu-id="190bb-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="190bb-115">Em seguida, preencha o texto do corpo usando o material de rascunho na seção Insights do Cliente da página regra de alquimia</span><span class="sxs-lookup"><span data-stu-id="190bb-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="190bb-116">Listas bulleted são muito bem</span><span class="sxs-lookup"><span data-stu-id="190bb-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="190bb-117">Listas numeradas também</span><span class="sxs-lookup"><span data-stu-id="190bb-117">Numbered lists too</span></span>
    1. <span data-ttu-id="190bb-118">**Negrito** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="190bb-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="190bb-119">Links devem ser sempre **"links para web" / externa** ou **links profundos para elementos**de ura, não links internos.</span><span class="sxs-lookup"><span data-stu-id="190bb-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="190bb-120">As imagens não são oficialmente suportadas neste momento, mas está no roteiro.</span><span class="sxs-lookup"><span data-stu-id="190bb-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="190bb-121">E isso já é realmente um pouco longo demais.</span><span class="sxs-lookup"><span data-stu-id="190bb-121">And this is really already a bit too long.</span></span> <span data-ttu-id="190bb-122">A melhor prática é de cerca de 400 personagens ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="190bb-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="190bb-123">Uma vez que seu conteúdo está pronto, puxá-lo para o ramo ao vivo.</span><span class="sxs-lookup"><span data-stu-id="190bb-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="190bb-124">Em seguida, vá para o [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) e digite o nome de arquivo no campo url.</span><span class="sxs-lookup"><span data-stu-id="190bb-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 