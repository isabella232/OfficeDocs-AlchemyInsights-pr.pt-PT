---
title: Conteúdo não aparece nos resultados da pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517042"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="58ffc-102">Conteúdo não aparece nos resultados da pesquisa do SharePoint</span><span class="sxs-lookup"><span data-stu-id="58ffc-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="58ffc-103">Siga estes passos de resolução de problemas quando conteúdo esperado não aparece nos resultados da procura:</span><span class="sxs-lookup"><span data-stu-id="58ffc-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="58ffc-104">Verifique se o **site** que contém o conteúdo esperado está definidas para permitir a apresentação nos resultados da pesquisa de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="58ffc-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="58ffc-105">Siga os passos de [Mostrar conteúdo num site nos resultados da procura](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="58ffc-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="58ffc-106">Verifique que a **lista** ou **biblioteca** que contém o conteúdo esperado está definido para permitir a apresentação nos resultados da pesquisa de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="58ffc-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="58ffc-107">Siga os passos de [Mostrar o conteúdo das listas ou bibliotecas nos resultados da procura](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="58ffc-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="58ffc-108">Certifique-se de que a página, documento ou esquema de página personalizada é publicada como uma **versão principal.**</span><span class="sxs-lookup"><span data-stu-id="58ffc-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="58ffc-109">Siga o passo 3 na [procura não devolver todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="58ffc-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="58ffc-110">Certifique-se de que o utilizador tem **permissões** para ver o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="58ffc-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="58ffc-111">Siga os passos nos [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="58ffc-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="58ffc-112">Se o esquema de pesquisa foi alterado adicionando uma nova propriedade gerida, através da edição de uma propriedade gerida ou removendo uma propriedade gerida, em seguida, pedir uma pesquisa e re-indexar será necessário.</span><span class="sxs-lookup"><span data-stu-id="58ffc-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="58ffc-113">**Re-indexar** o conteúdo seguindo os passos no [pedido manualmente de pesquisa e indexação voltar de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="58ffc-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="58ffc-114">Isto poderá demorar alguns minutos, aguarde 24 horas antes de verificar os resultados novamente.</span><span class="sxs-lookup"><span data-stu-id="58ffc-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="58ffc-115">Para mais informações, consulte [Activar o conteúdo de um site para ser procurado](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="58ffc-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
