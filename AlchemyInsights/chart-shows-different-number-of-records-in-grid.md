---
title: Gráfico mostra número diferente de registos na grelha
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439966"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Gráfico mostra número diferente de registos na grelha

**Sintoma**

Para gráfico na página do painel de instrumentos, quando clicar na tabela "..." e clique em "Ver registos", navegue na página da grelha para ver todos os registos. Às vezes, o número de registos muda.

**Causa**

Isto deve-se à diferença de pontos de vista entre o gráfico na página original do painel de instrumentos e o gráfico na página inicial da grelha.  

**Solução**

1. Verifique a vista da página original e a vista na grelha para ver se são diferentes.
2. Altere a vista na grelha para corresponder à vista na página original.
3. Se a vista correta não puder ser encontrada, geralmente significa que a vista não está ativada no designer de aplicações.
4. Vá ao designer de aplicações da aplicação específica, escolha a entidade e as suas opiniões, verifique a vista que pretende ativar, guardar, publicar e fechar.
5. Refresque a página.