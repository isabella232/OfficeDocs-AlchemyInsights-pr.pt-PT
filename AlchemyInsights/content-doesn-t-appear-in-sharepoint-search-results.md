---
title: O conteúdo não aparece nos resultados de pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713141"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="7843c-102">O conteúdo não aparece nos resultados de pesquisa do SharePoint</span><span class="sxs-lookup"><span data-stu-id="7843c-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="7843c-103">Siga estes passos de resolução de problemas quando o conteúdo esperado não aparece nos resultados da pesquisa:</span><span class="sxs-lookup"><span data-stu-id="7843c-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="7843c-104">Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7843c-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="7843c-105">Siga os passos em [Mostrar conteúdo num site em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="7843c-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="7843c-106">Verifique se a **lista** ou **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7843c-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="7843c-107">Siga os passos em [Mostrar conteúdo de listas ou bibliotecas em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="7843c-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="7843c-108">Verifique se a página, documento ou layout de página personalizada é publicado como uma **versão Major.**</span><span class="sxs-lookup"><span data-stu-id="7843c-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="7843c-109">Siga o passo 3 na [Search não devolva todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="7843c-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="7843c-110">Verifique se o utilizador tem **permissões** para visualizar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7843c-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="7843c-111">Siga os passos nos [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="7843c-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="7843c-112">Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerida, editando uma propriedade gerida, ou removendo uma propriedade gerida, então solicitar um rastreio e re-indexamento será necessário.</span><span class="sxs-lookup"><span data-stu-id="7843c-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="7843c-113">**Re-indexar** o conteúdo seguindo os passos em [Manualmente solicitar o rastreio e re-indexação de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="7843c-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="7843c-114">Isto pode demorar um pouco, esperar 24 horas antes de verificar os resultados novamente.</span><span class="sxs-lookup"><span data-stu-id="7843c-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="7843c-115">Para obter mais informações, consulte [Ativar o conteúdo de um site a pes pes que possa ser pes pes pesável.](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="7843c-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
