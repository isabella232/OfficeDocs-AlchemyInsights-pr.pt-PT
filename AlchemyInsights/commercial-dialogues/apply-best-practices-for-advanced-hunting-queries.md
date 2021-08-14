---
title: Aplicar práticas recomendadas para consultas de procura avançadas
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930144"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Aplicar práticas recomendadas para consultas de procura avançadas

Para obter resultados mais rapidamente e evitar tempos esgotados ao executar consultas complexas, aplique estas práticas recomendadas:

- Ao experimentar novas consultas, utilize sempre um limite para evitar obter conjuntos de resultados extremamente grandes. Além disso, `count` utilize para fazer uma avaliação inicial do tamanho do conjunto de resultados.
- Utilize filtros de tempo primeiro. Idealmente, limite as suas consultas a sete dias.
- No início de uma consulta, logo após o filtro de tempo, adicione os filtros esperados para remover a maior parte dos dados.
- Ao procurar tokens completos, utilize o `has` operador em vez de `contains` .
- Execute uma pesquisa numa coluna específica em vez de em todas as colunas.
- Ao associar tabelas, especifique primeiro a tabela com menos linhas.
- `project` apenas as colunas necessárias das tabelas a que aderiu.

Para saber mais, consulte [Práticas recomendadas de consulta avançada.](https://go.microsoft.com/fwlink/?linkid=2144812)
