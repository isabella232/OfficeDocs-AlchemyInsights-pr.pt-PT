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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510583"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="3a044-102">Pesquisa de conteúdo não devolvendo os resultados esperados</span><span class="sxs-lookup"><span data-stu-id="3a044-102">Content Search not returning expected results</span></span>

<span data-ttu-id="3a044-103">Ao executar pesquisas de conteúdo a partir do Microsoft 365 security & Compliance Center, poderá receber resultados de pesquisa inesperados.</span><span class="sxs-lookup"><span data-stu-id="3a044-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="3a044-104">Considere as seguintes coisas que podem afetar os seus resultados de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="3a044-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="3a044-105">**Localizações do conteúdo e condições de pesquisa**: Certifique-se de que selecionou as localizações e condições de pesquisa adequadas.</span><span class="sxs-lookup"><span data-stu-id="3a044-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="3a044-106">Se fez uma grande pesquisa (com muitas localizações), considere dividi-la em múltiplas pesquisas.</span><span class="sxs-lookup"><span data-stu-id="3a044-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="3a044-107">**Itens parcialmente indexados**: [Os itens parcialmente indexados](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) a partir de caixas de correio estão incluídos nos resultados de pesquisa estimados.</span><span class="sxs-lookup"><span data-stu-id="3a044-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="3a044-108">No entanto, itens parcialmente indexados de sites no SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="3a044-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="3a044-109">**Falhas de pesquisa**: Ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002).</span><span class="sxs-lookup"><span data-stu-id="3a044-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="3a044-110">Neste caso, recandiduzem a procura apenas para as localizações de conteúdo falhado.</span><span class="sxs-lookup"><span data-stu-id="3a044-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="3a044-111">Consulte [este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="3a044-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
