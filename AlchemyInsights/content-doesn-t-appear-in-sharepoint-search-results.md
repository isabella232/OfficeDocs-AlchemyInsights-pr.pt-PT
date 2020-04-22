---
title: Conteúdo não aparece nos resultados de pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705672"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="b1f45-102">Conteúdo não aparece nos resultados de pesquisa do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b1f45-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="b1f45-103">Siga estes passos de resolução de problemas quando o conteúdo esperado não aparece nos resultados da pesquisa:</span><span class="sxs-lookup"><span data-stu-id="b1f45-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="b1f45-104">Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b1f45-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="b1f45-105">Siga os passos em [Mostrar conteúdo num site em resultados](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)de pesquisa .</span><span class="sxs-lookup"><span data-stu-id="b1f45-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="b1f45-106">Verifique se a **lista** ou **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b1f45-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="b1f45-107">Siga os passos em [Mostrar conteúdo de listas ou bibliotecas em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="b1f45-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="b1f45-108">Verifique se a página, documento ou layout de página personalizado é publicado como uma **versão Major.**</span><span class="sxs-lookup"><span data-stu-id="b1f45-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="b1f45-109">Siga o passo 3 em [Search não devolve todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="b1f45-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="b1f45-110">Verifique se o utilizador tem **permissões** para visualizar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b1f45-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="b1f45-111">Siga os passos em compreender os níveis de [permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="b1f45-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="b1f45-112">Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerida, editando uma propriedade gerida, ou removendo uma propriedade gerida, então será necessário solicitar um rastreio e um re-indexante.</span><span class="sxs-lookup"><span data-stu-id="b1f45-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="b1f45-113">**Reindexe** o conteúdo seguindo os passos em [manualmente solicitar rastejar e reindexar um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="b1f45-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="b1f45-114">Isto pode demorar um pouco, espere 24 horas antes de verificar novamente os resultados.</span><span class="sxs-lookup"><span data-stu-id="b1f45-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="b1f45-115">Para mais informações, consulte [Ativar o conteúdo num site para ser pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b1f45-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
