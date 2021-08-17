---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052721"
---
# <a name="content-search-not-returning-expected-results"></a>A Pesquisa de Conteúdos não devolve os resultados esperados

Ao executar Pesquisas de Conteúdo a partir do centro Microsoft 365 de & Conformidade, poderá receber resultados de pesquisa inesperados. Considere as seguintes coisas que podem afetar os resultados da sua pesquisa:

- **Localizações de conteúdo e condições de pesquisa:** certifique-se de que selecionou as localizações de conteúdo adequadas e as condições de pesquisa. Se tiver enalteado uma pesquisa grande (com muitas localizações), considere dividi-la em múltiplas pesquisas.

- **Itens parcialmente indexados:**  [os itens parcialmente indexados](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) das caixas de correio são incluídos nos resultados estimados da pesquisa. No entanto, os itens parcialmente indexados de sites no SharePoint OneDrive não são incluídos na estimativa de pesquisa.

- **Falhas** de pesquisa: ao procurar um grande número de caixas de correio (mais de 100.000 caixas de correio), poderá obter erros de pesquisa, com códigos de erro como CS008-009 e CS012-002). Neste caso, re repetir a pesquisa apenas para as localizações de conteúdos falhadas. Consulte  [este artigo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obter mais informações.
