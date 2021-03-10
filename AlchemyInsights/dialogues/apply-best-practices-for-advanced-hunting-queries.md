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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696087"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Aplicar as melhores práticas para consultas avançadas de caça

Para obter resultados mais rápidos e para evitar intervalos de tempo enquanto executa consultas complexas, aplique estas melhores práticas:

- Ao experimentar novas consultas, use sempre um limite, para evitar obter conjuntos de resultados extremamente grandes. Além disso, utilize `count` para fazer uma avaliação inicial do tamanho do conjunto de resultados.
- Utilize primeiro os filtros de tempo. Idealmente, limite as suas consultas a sete dias.
- No início de uma consulta, logo após o filtro de tempo, adicione os filtros esperados para remover a maioria dos dados.
- Quando procurar fichas completas, utilize o `has` operador em vez de `contains` .
- Procure numa coluna específica e não em todas as colunas.
- Ao juntar mesas, primeiro especifique a tabela com menos filas.
- `project` apenas as colunas necessárias das mesas a que se juntou.

Para saber mais, consulte [as melhores práticas de consulta de caça avançada.](https://go.microsoft.com/fwlink/?linkid=2144812)
