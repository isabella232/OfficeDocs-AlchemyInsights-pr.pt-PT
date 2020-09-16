---
title: Gerir esquema de pesquisa no SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770562"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="477d4-102">Gerir esquema de pesquisa no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="477d4-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="477d4-103">O esquema de pesquisa controla o que os utilizadores podem pesquisar, como os utilizadores podem pesquisar e como pode apresentar os resultados nos seus sites de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="477d4-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="477d4-104">Consulte [gerir o esquema de pesquisa no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) para aprender a:</span><span class="sxs-lookup"><span data-stu-id="477d4-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="477d4-105">Mude o esquema de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="477d4-105">Change the search schema.</span></span>
- <span data-ttu-id="477d4-106">Criar propriedades geridas.</span><span class="sxs-lookup"><span data-stu-id="477d4-106">Create managed properties.</span></span>
- <span data-ttu-id="477d4-107">Mapa rastejado de propriedades rastejadas para propriedades geridas.</span><span class="sxs-lookup"><span data-stu-id="477d4-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="477d4-108">Note o seguinte no que diz respeito à gestão do seu Esquema de Pesquisa:</span><span class="sxs-lookup"><span data-stu-id="477d4-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="477d4-109">Se receber um aviso indicando que **a aplicação é interrompida** ao fazer uma alteração de esquema, esta é apenas temporária, uma vez que existe manutenção de serviço.</span><span class="sxs-lookup"><span data-stu-id="477d4-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="477d4-110">Se já passaram mais de 24 horas e ainda experimenta o aviso, por favor registe um caso de apoio.</span><span class="sxs-lookup"><span data-stu-id="477d4-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="477d4-111">Quando altera propriedades geridas ou adiciona novas, as alterações só têm efeito depois de o conteúdo ter sido re-rastejado.</span><span class="sxs-lookup"><span data-stu-id="477d4-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="477d4-112">No SharePoint Online, o rastreio acontece automaticamente com base no horário definido de rastreio.</span><span class="sxs-lookup"><span data-stu-id="477d4-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="477d4-113">Para se certificar de que as suas alterações estão rastreadas, pode solicitar especificamente [uma re-indexação da lista ou biblioteca](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="477d4-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="477d4-114">Para uma visão geral completa do Esquema de Pesquisa, consulte [a introdução do esquema de pesquisa](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="477d4-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


