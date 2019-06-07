---
title: Gerir dicionários de procura no SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758776"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="06301-102">Procurar no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="06301-102">Search in SharePoint Online</span></span>

<span data-ttu-id="06301-103">Conteúdo deve ser pesquisado e adicionado ao índice de procura aos utilizadores a localização daquilo procura no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="06301-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="06301-104">Conteúdo é pesquisado automaticamente com base numa agenda de pesquisa predefinido (não é possível alterar a agenda de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="06301-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="06301-105">O crawler capta conteúdo que foi alterado desde a última pesquisa e actualiza o índice.</span><span class="sxs-lookup"><span data-stu-id="06301-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="06301-106">Para garantir o conteúdo é pesquisado e o índice é actualizado, siga os passos abaixo.</span><span class="sxs-lookup"><span data-stu-id="06301-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="06301-107">Certifique-se de conteúdo pode ser encontrado, tornando o conteúdo do site pesquisável.</span><span class="sxs-lookup"><span data-stu-id="06301-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="06301-108">Para obter mais informações, consulte [Activar o conteúdo de um site para ser procurado](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="06301-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="06301-109">Quando alterar uma propriedade gerida ou quando alterou o mapeamento de pesquisado e geridos propriedades, o site tem de ser novamente pesquisadas antes das alterações serão reflectidas no índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="06301-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="06301-110">Uma vez que as alterações serão efectuadas no esquema de procura e não para o site actual, o crawler não adicionará automaticamente re-indexe o site.</span><span class="sxs-lookup"><span data-stu-id="06301-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="06301-111">Para obter mais informações, consulte [Pedir manualmente de pesquisa e indexação voltar de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="06301-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="06301-112">Aguarde, pelo menos, 24 horas após solicitar manualmente uma pesquisa e, em seguida, completa reindexar para ver se ainda estiver com um problema.</span><span class="sxs-lookup"><span data-stu-id="06301-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="06301-113">Se tiverem passado mais de 24 horas desde que iniciou a pesquisa e, em seguida, reindexar completo, inicie a sessão de um incidente de suporte.</span><span class="sxs-lookup"><span data-stu-id="06301-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="06301-114">Em muitos casos, a Microsoft já estiver a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="06301-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="06301-115">Forneça pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="06301-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="06301-116">**Importante**: se um site, o documento (biblioteca) ou uma lista foi eliminada e ainda mostra nos resultados da procura, os utilizadores devem receber um erro 404 ficheiro não encontrado quando tentar aceder.</span><span class="sxs-lookup"><span data-stu-id="06301-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="06301-117">Este problema deve ser registado como um incidente de suporte para a investigação suplementar.</span><span class="sxs-lookup"><span data-stu-id="06301-117">This issue should be logged as a support case for further investigation.</span></span> 



