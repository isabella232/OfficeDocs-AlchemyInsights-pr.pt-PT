---
title: mesmo que o nome do arquivo é melhor
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800056"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="34a7d-102">Cabeçalho de alquimia obrigatório H1, H2's não funciona.</span><span class="sxs-lookup"><span data-stu-id="34a7d-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="34a7d-103">Melhores práticas e diretrizes para criação de alquimia:</span><span class="sxs-lookup"><span data-stu-id="34a7d-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="34a7d-104">**Não aninhar o Alchemy insights em pastas**-isso quebrará a estrutura de URL.</span><span class="sxs-lookup"><span data-stu-id="34a7d-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="34a7d-105">Estamos procurando consertar isso.</span><span class="sxs-lookup"><span data-stu-id="34a7d-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="34a7d-106">Os arquivos na pasta **Alchemyinsights** devem ter nomes de arquivo minúsculos com hífens para espaços ex.</span><span class="sxs-lookup"><span data-stu-id="34a7d-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="34a7d-107">***How-to-Enable-litígio-Hold***.</span><span class="sxs-lookup"><span data-stu-id="34a7d-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="34a7d-108">Inclua o ID da regra ou o ID do Bucket no [portal do parceiro de alquimia](https://alchemyportal.azurewebsites.net) no campo MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="34a7d-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="34a7d-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="34a7d-109">ex.</span></span> <span data-ttu-id="34a7d-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="34a7d-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="34a7d-111">Use o restante dos metadados na parte superior deste arquivo como seu modelo.</span><span class="sxs-lookup"><span data-stu-id="34a7d-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="34a7d-112">No [portal do parceiro de alquimia](https://alchemyportal.azurewebsites.net), navegue até a seção **título do cliente Insight:** e use isso como um ponto de partida para o seu título H1 para o Insight.</span><span class="sxs-lookup"><span data-stu-id="34a7d-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="34a7d-113">O Alchemy insights deve ter apenas um único H1 na parte superior ou eles quebrarão na produção.</span><span class="sxs-lookup"><span data-stu-id="34a7d-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="34a7d-114">O H2S não renderiza tanto o uso de convenções **Bold** ou Other para significar seções separadas.</span><span class="sxs-lookup"><span data-stu-id="34a7d-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="34a7d-115">Em seguida, preencha o texto do corpo usando o material de rascunho na seção insights do cliente da página regra de alquimia</span><span class="sxs-lookup"><span data-stu-id="34a7d-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="34a7d-116">Listas com marcadores estão bem</span><span class="sxs-lookup"><span data-stu-id="34a7d-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="34a7d-117">Listas numeradas também</span><span class="sxs-lookup"><span data-stu-id="34a7d-117">Numbered lists too</span></span>
    1. <span data-ttu-id="34a7d-118">**Negrito** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="34a7d-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="34a7d-119">Links devem ser sempre **"links para Web"/External** ou **Deep-links para elementos de interface do usuário**, não links internos.</span><span class="sxs-lookup"><span data-stu-id="34a7d-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="34a7d-120">As imagens não são oficialmente suportadas neste momento, mas é sobre o roteiro.</span><span class="sxs-lookup"><span data-stu-id="34a7d-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="34a7d-121">E isso já é um pouco longo demais.</span><span class="sxs-lookup"><span data-stu-id="34a7d-121">And this is really already a bit too long.</span></span> <span data-ttu-id="34a7d-122">A melhor prática é de cerca de 400 caracteres---------------------------------</span><span class="sxs-lookup"><span data-stu-id="34a7d-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="34a7d-123">Quando o conteúdo estiver pronto, puxe-o para a ramificação ao vivo.</span><span class="sxs-lookup"><span data-stu-id="34a7d-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="34a7d-124">Em seguida, vá para o [portal do parceiro de alquimia](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo URL.</span><span class="sxs-lookup"><span data-stu-id="34a7d-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 