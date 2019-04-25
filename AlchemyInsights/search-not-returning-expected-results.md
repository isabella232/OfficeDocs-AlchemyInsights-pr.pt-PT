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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383846"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="a4b04-102">Pesquisa de conteúdo não devolver os resultados esperados</span><span class="sxs-lookup"><span data-stu-id="a4b04-102">Content Search not returning expected results</span></span>

<span data-ttu-id="a4b04-103">Quando executar procuras de conteúdo a partir do & de segurança do Office 365 Centro de conformidade, poderá receber resultados inesperados.</span><span class="sxs-lookup"><span data-stu-id="a4b04-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="a4b04-104">Considere as seguintes acções que podem afectar os resultados da pesquisa:</span><span class="sxs-lookup"><span data-stu-id="a4b04-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="a4b04-105">**Localizações de conteúdo e as condições de procura**: Certifique-se de que seleccionou as localizações de conteúdo correctas e as condições de procura.</span><span class="sxs-lookup"><span data-stu-id="a4b04-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="a4b04-106">Se executar uma procura de grandes dimensões (com várias localizações), considere dividi-la em várias procuras.</span><span class="sxs-lookup"><span data-stu-id="a4b04-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="a4b04-107">**Itens indexados parcialmente**: [parcialmente indexados itens](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas de correio estão incluídos nos resultados da procura estimado.</span><span class="sxs-lookup"><span data-stu-id="a4b04-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="a4b04-108">No entanto, os itens indexados parcialmente de sites SharePoint e OneDrive não são incluídos na estimativa de procura.</span><span class="sxs-lookup"><span data-stu-id="a4b04-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="a4b04-109">**Falhas de procura**: quando procura um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de procura, com códigos de erro, tais como CS008-009 e CS012-002).</span><span class="sxs-lookup"><span data-stu-id="a4b04-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="a4b04-110">Neste caso, tente novamente a procura apenas para as localizações de conteúdo falhou.</span><span class="sxs-lookup"><span data-stu-id="a4b04-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="a4b04-111">Consulte [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a4b04-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
