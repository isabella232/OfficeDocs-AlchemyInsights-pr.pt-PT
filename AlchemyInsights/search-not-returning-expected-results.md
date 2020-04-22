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
# <a name="content-search-not-returning-expected-results"></a>Pesquisa de conteúdo não devolve resultados esperados

Ao executar as pesquisas de conteúdo do Microsoft 365 security & Compliance Center, poderá receber resultados de pesquisa inesperados. Considere as seguintes coisas que podem afetar os resultados da sua pesquisa:

- Localização de **conteúdo e condições**de pesquisa : Certifique-se de que selecionou os locais de conteúdo adequados e as condições de pesquisa. Se fez uma grande pesquisa (com muitos locais), considere dividi-la em múltiplas pesquisas.

- **Itens parcialmente indexados**: [Os itens parcialmente indexados](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas de correio estão incluídos nos resultados de pesquisa estimados. No entanto, itens parcialmente indexados de sites em SharePoint e OneDrive não estão incluídos na estimativa de pesquisa.

- **Falhas de pesquisa**: Ao pesquisar um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Neste caso, tente novamente a procura apenas pelos locais de conteúdo falhados. Consulte [este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para mais informações.
