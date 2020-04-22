---
title: 1491-pesquisa-não-retorno-resultados esperados
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709238"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="2ba99-102">Pesquisa de conteúdo não devolve resultados esperados</span><span class="sxs-lookup"><span data-stu-id="2ba99-102">Content Search not returning expected results</span></span>

<span data-ttu-id="2ba99-103">Ao executar as pesquisas de conteúdo do Microsoft 365 security & Compliance Center, poderá receber resultados de pesquisa inesperados.</span><span class="sxs-lookup"><span data-stu-id="2ba99-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="2ba99-104">Considere as seguintes coisas que podem afetar os resultados da sua pesquisa:</span><span class="sxs-lookup"><span data-stu-id="2ba99-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="2ba99-105">Localização de **conteúdo e condições**de pesquisa : Certifique-se de que selecionou os locais de conteúdo adequados e as condições de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2ba99-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="2ba99-106">Se fez uma grande pesquisa (com muitos locais), considere dividi-la em múltiplas pesquisas.</span><span class="sxs-lookup"><span data-stu-id="2ba99-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="2ba99-107">**Itens parcialmente indexados**: [Os itens parcialmente indexados](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas de correio estão incluídos nos resultados de pesquisa estimados.</span><span class="sxs-lookup"><span data-stu-id="2ba99-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="2ba99-108">No entanto, itens parcialmente indexados de sites em SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2ba99-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="2ba99-109">**Falhas de pesquisa**: Ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002).</span><span class="sxs-lookup"><span data-stu-id="2ba99-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="2ba99-110">Neste caso, tente novamente a procura apenas pelos locais de conteúdo falhados.</span><span class="sxs-lookup"><span data-stu-id="2ba99-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="2ba99-111">Consulte [este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="2ba99-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
