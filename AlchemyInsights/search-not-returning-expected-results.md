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
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551426"
---
# <a name="content-search-not-returning-expected-results"></a>Pesquisa de conteúdo não devolver os resultados esperados

Quando executar procuras de conteúdo a partir do & de segurança do Office 365 Centro de conformidade, poderá receber resultados inesperados. Considere as seguintes acções que podem afectar os resultados da pesquisa:

- **Localizações de conteúdo e as condições de procura**: Certifique-se de que seleccionou as localizações de conteúdo correctas e as condições de procura. Se executar uma procura de grandes dimensões (com várias localizações), considere dividi-la em várias procuras.

- **Itens indexados parcialmente**: [parcialmente indexados itens](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas de correio estão incluídos nos resultados da procura estimado. No entanto, os itens indexados parcialmente de sites SharePoint e OneDrive não são incluídos na estimativa de procura.

- **Falhas de procura**: quando procura um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de procura, com códigos de erro, tais como CS008-009 e CS012-002). Neste caso, tente novamente a procura apenas para as localizações de conteúdo falhou. Consulte [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.
