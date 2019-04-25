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
# <a name="content-search-not-returning-expected-results"></a>Pesquisa de conteúdo não devolver os resultados esperados

Quando executar procuras de conteúdo a partir do & de segurança do Office 365 Centro de conformidade, poderá receber resultados inesperados. Considere as seguintes acções que podem afectar os resultados da pesquisa:

- **Localizações de conteúdo e as condições de procura**: Certifique-se de que seleccionou as localizações de conteúdo correctas e as condições de procura. Se executar uma procura de grandes dimensões (com várias localizações), considere dividi-la em várias procuras.

- **Itens indexados parcialmente**: [parcialmente indexados itens](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) das caixas de correio estão incluídos nos resultados da procura estimado. No entanto, os itens indexados parcialmente de sites SharePoint e OneDrive não são incluídos na estimativa de procura.

- **Falhas de procura**: quando procura um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de procura, com códigos de erro, tais como CS008-009 e CS012-002). Neste caso, tente novamente a procura apenas para as localizações de conteúdo falhou. Consulte [Este artigo](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) para obter mais informações.
