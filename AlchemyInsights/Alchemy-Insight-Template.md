---
title: mesmo que nome de arquivo é melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750981"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Cabeçalho de Alquimia H1, H2 não funciona."
Boas Práticas e orientações para a autoria da Alquimia:

1. **Não aninhar a Alquimia Insights em pastas**- isto quebrará a estrutura url. Estamos a tentar resolver isto.
1. Os ficheiros na pasta **AlchemyInsights** devem ter canções minúsculas com hífenes para espaços ex. ***como permitir-permitir litígios- hold***.
    1. Inclua o ID de Regra ou ID do balde do [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) no campo ms.custom. ex. ***ms.custom: 100021***
1. Utilize o resto dos metadados na parte superior deste ficheiro como modelo.
1. No [portal Alchemy Partner,](https://alchemyportal.azurewebsites.net)navegue até à secção **Título de Insight do Cliente:** e use-o como ponto de partida para o seu título H1 para a visão. 
    > [!NOTE]
    > A Alquimia Insights DEVE ter apenas um H1 no topo ou eles vão quebrar a produção. Os H2 não prestam nem por isso usam convenções **ousadas** ou outras para significar secções separadas.
1. Em seguida, preencha o texto do corpo utilizando o material de projeto na secção de Insights do Cliente da página Regra da Alquimia
    1. As listas de balas estão bem.
    1. Listas numeradas também
    1. **Arrojado** e *itálico* são a-ok
    1. As ligações devem ser sempre **"links para web"/external** OU **ligações profundas a elementos de UI,** e não ligações internas.
    1. As fotos não são oficialmente suportadas neste momento, mas está no roteiro.

E isto já é um pouco longo demais. A melhor prática é cerca de 400 caracteres ---------------------------------

Assim que o seu conteúdo estiver pronto, puxe-o para o ramo ao vivo. Em seguida, vá ao [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) e introduza o nome de arquivo no campo url. 