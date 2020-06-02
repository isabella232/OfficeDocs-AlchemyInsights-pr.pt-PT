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
# <a name="content-search-not-returning-expected-results"></a>Pesquisa de conteúdo não devolvendo os resultados esperados

Ao executar pesquisas de conteúdo a partir do Microsoft 365 security & Compliance Center, poderá receber resultados de pesquisa inesperados. Considere as seguintes coisas que podem afetar os seus resultados de pesquisa:

- **Localizações do conteúdo e condições de pesquisa**: Certifique-se de que selecionou as localizações e condições de pesquisa adequadas. Se fez uma grande pesquisa (com muitas localizações), considere dividi-la em múltiplas pesquisas.

- **Itens parcialmente indexados**: [Os itens parcialmente indexados](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) a partir de caixas de correio estão incluídos nos resultados de pesquisa estimados. No entanto, itens parcialmente indexados de sites no SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.

- **Falhas de pesquisa**: Ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Neste caso, recandiduzem a procura apenas para as localizações de conteúdo falhado. Consulte [este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para mais informações.
