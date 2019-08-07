---
title: Procurar no SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059263"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="af4f0-102">Procurar no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="af4f0-102">Search in SharePoint Online</span></span>

<span data-ttu-id="af4f0-103">Conteúdo deve ser pesquisado e adicionado ao índice de procura aos utilizadores a localização daquilo procura no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="af4f0-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="af4f0-104">Conteúdo é pesquisado automaticamente com base numa agenda de pesquisa predefinido (não é possível alterar a agenda de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="af4f0-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="af4f0-105">O crawler capta conteúdo que foi alterado desde a última pesquisa e actualiza o índice.</span><span class="sxs-lookup"><span data-stu-id="af4f0-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="af4f0-106">Para garantir o conteúdo é pesquisado e o índice é actualizado, tenha em atenção o seguinte:</span><span class="sxs-lookup"><span data-stu-id="af4f0-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="af4f0-107">Certifique-se de conteúdo pode ser encontrado, [tornando o conteúdo do site pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="af4f0-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="af4f0-108">Quando alterar uma propriedade gerida ou quando alterou o mapeamento de pesquisado e geridos propriedades, o site tem de ser novamente pesquisadas antes das alterações serão reflectidas no índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="af4f0-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="af4f0-109">Uma vez que as alterações serão efectuadas no esquema de procura e não para o site actual, o crawler não adicionará automaticamente re-indexe o site.</span><span class="sxs-lookup"><span data-stu-id="af4f0-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="af4f0-110">Para obter mais informações, consulte [Pedir manualmente de pesquisa e indexação voltar de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="af4f0-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="af4f0-111">Aguarde, pelo menos, 24 horas após solicitar manualmente uma pesquisa e, em seguida, completa reindexar para ver se ainda estiver com um problema.</span><span class="sxs-lookup"><span data-stu-id="af4f0-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="af4f0-112">Se tiverem passado mais de 24 horas desde que iniciou a pesquisa e, em seguida, reindexar completo, inicie a sessão de um incidente de suporte.</span><span class="sxs-lookup"><span data-stu-id="af4f0-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="af4f0-113">Em muitos casos, a Microsoft já estiver a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="af4f0-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="af4f0-114">Forneça pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="af4f0-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Importante!]<span data-ttu-id="af4f0-115">: se um site, o documento (biblioteca) ou uma lista foi eliminada e ainda mostra nos resultados da procura, os utilizadores devem receber um **Erro 404 ficheiro não encontrado** ao tentar aceder a ele.</span><span class="sxs-lookup"><span data-stu-id="af4f0-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="af4f0-116">Este problema deve ser registado como um incidente de suporte para a investigação suplementar.</span><span class="sxs-lookup"><span data-stu-id="af4f0-116">This issue should be logged as a support case for further investigation.</span></span> 



