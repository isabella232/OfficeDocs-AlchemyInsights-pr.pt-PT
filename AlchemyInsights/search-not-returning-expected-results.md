---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355888"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="94258-102">Pesquisa de conteúdo não devolver os resultados esperados</span><span class="sxs-lookup"><span data-stu-id="94258-102">Content Search not returning expected results</span></span>

<span data-ttu-id="94258-103">Quando executar procuras de conteúdo a partir do & de segurança do Office 365 Centro de conformidade, poderá receber resultados inesperados.</span><span class="sxs-lookup"><span data-stu-id="94258-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="94258-104">Considere as seguintes acções que podem afectar os resultados da pesquisa:</span><span class="sxs-lookup"><span data-stu-id="94258-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="94258-105">**Localizações de conteúdo e as condições de procura**: Certifique-se de que seleccionou as localizações de conteúdo correctas e as condições de procura.</span><span class="sxs-lookup"><span data-stu-id="94258-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="94258-106">Se executar uma procura de grandes dimensões (com várias localizações), considere dividi-la em várias procuras.</span><span class="sxs-lookup"><span data-stu-id="94258-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="94258-107">**Itens indexados parcialmente**: [parcialmente indexados itens](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas de correio estão incluídos nos resultados da procura estimado.</span><span class="sxs-lookup"><span data-stu-id="94258-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="94258-108">No entanto, os itens indexados parcialmente de sites SharePoint e OneDrive não são incluídos na estimativa de procura.</span><span class="sxs-lookup"><span data-stu-id="94258-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="94258-109">**Falhas de procura**: quando procura um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de procura, com códigos de erro, tais como CS008-009 e CS012-002).</span><span class="sxs-lookup"><span data-stu-id="94258-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="94258-110">Neste caso, tente novamente a procura apenas para as localizações de conteúdo falhou.</span><span class="sxs-lookup"><span data-stu-id="94258-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="94258-111">Consulte [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="94258-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
