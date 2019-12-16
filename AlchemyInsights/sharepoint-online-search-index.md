---
title: Pesquisa no SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044054"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="59826-102">Rastreamento de conteúdo e indexação no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="59826-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="59826-103">O conteúdo deve ser rastreado e adicionado ao índice de pesquisa para que os usuários encontrem o que estão pesquisando no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="59826-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="59826-104">O conteúdo é automaticamente rastreado com base em um cronograma de rastreamento pré-definido (o cronograma de rastreamento não pode ser alterado).</span><span class="sxs-lookup"><span data-stu-id="59826-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="59826-105">O rastreador capta conteúdo que mudou desde o último rastreamento e atualiza o índice.</span><span class="sxs-lookup"><span data-stu-id="59826-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="59826-106">Para garantir que o conteúdo seja rastreado e o índice seja atualizado, observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="59826-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="59826-107">Certifique-se de que o conteúdo pode ser encontrado tornando o conteúdo do [site pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="59826-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="59826-108">Quando você mudou uma propriedade controlada, ou quando você mudou o mapeamento de propriedades rastejadas e controladas, o local deve ser re-rastejado antes que suas mudanças sejam refletidas no índice da busca.</span><span class="sxs-lookup"><span data-stu-id="59826-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="59826-109">Como suas alterações são feitas no esquema de pesquisa e não no site real, o rastreador não reindexará automaticamente o site.</span><span class="sxs-lookup"><span data-stu-id="59826-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="59826-110">Para mais informações, consulte [manualmente rastreamento e re-indexação de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="59826-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="59826-111">Espere pelo menos 24 horas depois de solicitar manualmente um rastreamento e re-índice completo para ver se você ainda está enfrentando um problema.</span><span class="sxs-lookup"><span data-stu-id="59826-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="59826-112">Se mais de 24 horas se passaram desde que você iniciou o rastreamento e re-índice completo, por favor, registre um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="59826-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="59826-113">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="59826-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="59826-114">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="59826-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="59826-115">Se um site, documento (biblioteca) ou uma lista for excluído e ainda for exibido nos resultados da pesquisa, os usuários devem receber um **arquivo Erro 404 não encontrado** ao tentar acessá-lo.</span><span class="sxs-lookup"><span data-stu-id="59826-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="59826-116">Esta questão deve ser registrada como um caso de apoio para uma investigação mais aprofundada.</span><span class="sxs-lookup"><span data-stu-id="59826-116">This issue should be logged as a support case for further investigation.</span></span> 



