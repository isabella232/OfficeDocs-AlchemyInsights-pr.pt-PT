---
title: Aplicar as melhores práticas para consultas avançadas de caça
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749545"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="19a74-102">Aplicar as melhores práticas para consultas avançadas de caça</span><span class="sxs-lookup"><span data-stu-id="19a74-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="19a74-103">Para obter resultados mais rápidos e para evitar intervalos de tempo enquanto executa consultas complexas, aplique estas melhores práticas:</span><span class="sxs-lookup"><span data-stu-id="19a74-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="19a74-104">Ao experimentar novas consultas, use sempre um limite, para evitar obter conjuntos de resultados extremamente grandes.</span><span class="sxs-lookup"><span data-stu-id="19a74-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="19a74-105">Além disso, utilize `count` para fazer uma avaliação inicial do tamanho do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="19a74-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="19a74-106">Utilize primeiro os filtros de tempo.</span><span class="sxs-lookup"><span data-stu-id="19a74-106">Use time filters first.</span></span> <span data-ttu-id="19a74-107">Idealmente, limite as suas consultas a sete dias.</span><span class="sxs-lookup"><span data-stu-id="19a74-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="19a74-108">No início de uma consulta, logo após o filtro de tempo, adicione os filtros esperados para remover a maioria dos dados.</span><span class="sxs-lookup"><span data-stu-id="19a74-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="19a74-109">Quando procurar fichas completas, utilize o `has` operador em vez de `contains` .</span><span class="sxs-lookup"><span data-stu-id="19a74-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="19a74-110">Procure numa coluna específica e não em todas as colunas.</span><span class="sxs-lookup"><span data-stu-id="19a74-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="19a74-111">Ao juntar mesas, primeiro especifique a tabela com menos filas.</span><span class="sxs-lookup"><span data-stu-id="19a74-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="19a74-112">`project` apenas as colunas necessárias das mesas a que se juntou.</span><span class="sxs-lookup"><span data-stu-id="19a74-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="19a74-113">Para saber mais, consulte [as melhores práticas de consulta de caça avançada.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="19a74-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
