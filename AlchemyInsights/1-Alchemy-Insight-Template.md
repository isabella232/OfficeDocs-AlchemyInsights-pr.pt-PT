---
title: 'mesmo que o nome de ficheiro é melhor [regra #-descrição]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634515"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="f1964-102">Necessário Alquimia cabeçalho H1, H2 não funcionam.</span><span class="sxs-lookup"><span data-stu-id="f1964-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="f1964-103">Procedimentos recomendados e orientações para a criação de Alquimia:</span><span class="sxs-lookup"><span data-stu-id="f1964-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="f1964-104">**Não se aninham conhecimentos aprofundados de Alquimia em pastas**- Isto irá interromper a estrutura de URLs.</span><span class="sxs-lookup"><span data-stu-id="f1964-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="f1964-105">Procuramos, para corrigir isto.</span><span class="sxs-lookup"><span data-stu-id="f1964-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="f1964-106">Ficheiros na pasta **AlchemyInsights** devem ter o ID da regra e o nome da regra a partir do [portal para parceiros de Alquimia](https://alchemyportal.azurewebsites.net) no nome de ficheiro.</span><span class="sxs-lookup"><span data-stu-id="f1964-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="f1964-107">ex.</span><span class="sxs-lookup"><span data-stu-id="f1964-107">ex.</span></span> <span data-ttu-id="f1964-108">***976-How-to-Enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="f1964-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="f1964-109">Utilize os metadados na parte superior deste ficheiro como modelo.</span><span class="sxs-lookup"><span data-stu-id="f1964-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="f1964-110">Nada mais é necessário.</span><span class="sxs-lookup"><span data-stu-id="f1964-110">Nothing else is required.</span></span>
1. <span data-ttu-id="f1964-111">No [portal para parceiros de Alquimia](https://alchemyportal.azurewebsites.net), navegue para a secção **cliente Insight título:** e a utilização que, como um iniciar, aponte para o título H1 para a visão.</span><span class="sxs-lookup"><span data-stu-id="f1964-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="f1964-112">Alquimia informações privilegiadas deve ter apenas um único H1 na parte superior ou vão quebrar na produção.</span><span class="sxs-lookup"><span data-stu-id="f1964-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="f1964-113">H2s não compor assim utilização **negrito** ou outras convenções para significar secções separadas.</span><span class="sxs-lookup"><span data-stu-id="f1964-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="f1964-114">Em seguida, preencha o corpo de texto utilizando o material de projecto na secção informações de cliente da página regra de Alquimia</span><span class="sxs-lookup"><span data-stu-id="f1964-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="f1964-115">Listas com marcas estão correctos</span><span class="sxs-lookup"><span data-stu-id="f1964-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="f1964-116">Listas numeradas demasiado</span><span class="sxs-lookup"><span data-stu-id="f1964-116">Numbered lists too</span></span>
    1. <span data-ttu-id="f1964-117">**Negrito** e *itálico* são a-ok</span><span class="sxs-lookup"><span data-stu-id="f1964-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="f1964-118">Hiperligações devem ser sempre quer **"ligações Web" / externo** ou **deep-hiperligações para elementos da IU**, as hiperligações não internas.</span><span class="sxs-lookup"><span data-stu-id="f1964-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="f1964-119">E realmente já é um pouco demasiado longo.</span><span class="sxs-lookup"><span data-stu-id="f1964-119">And this is really already a bit too long.</span></span> <span data-ttu-id="f1964-120">Recomenda-se cerca de 400 caracteres--</span><span class="sxs-lookup"><span data-stu-id="f1964-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="f1964-121">Depois do conteúdo estiver pronto, puxe-lo para o ramo vivo.</span><span class="sxs-lookup"><span data-stu-id="f1964-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="f1964-122">Em seguida, vá para o [portal de parceiro de Alquimia](https://alchemyportal.azurewebsites.net) e introduza o nome de ficheiro para o campo de url.</span><span class="sxs-lookup"><span data-stu-id="f1964-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="f1964-123">Certifique-se de conhecimentos aprofundados revistas e publicadas indicar "Sim" e, em seguida, faça clique sobre a regra de actualização.</span><span class="sxs-lookup"><span data-stu-id="f1964-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="f1964-124">**(Esta procura prettier na nova versão do portal - logo que a libertação.)** 
 ![campo url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="f1964-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

