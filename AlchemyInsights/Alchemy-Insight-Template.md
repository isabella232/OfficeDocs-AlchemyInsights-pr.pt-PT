---
title: mesmo que o nome de ficheiro é o melhor
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
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676544"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Exigia alquimia cabeçalho H1, H2's não funciona.
Boas Práticas e orientações para a autoria da Alquimia:

1. **Não nidique alquimia insights em pastas**- isto quebrará a estrutura do url. Estamos a tentar resolver isto.
1. Os ficheiros na pasta **AlchemyInsights** devem ter nomes de ficheiros minúsculos com hífens para espaços ex. ***como permitir-ativar-contencioso-hold***.
    1. Inclua o ID de regra ou id balde do [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) no campo ms.custom. ex. ***ms.custom: 100021***
1. Utilize o resto dos metadados na parte superior deste ficheiro como modelo.
1. No [portal Alchemy Partner,](https://alchemyportal.azurewebsites.net)navegue até à secção Título de Insight do **Cliente:** e use-o como ponto de partida para o seu título de H1 para a insight. 
    > [!NOTE]
    > Alquimia Insights MUST tem apenas um único H1 no topo ou eles vão quebrar na produção. Os H2 não prestam nem por isso use convenções **ousadas** ou outras para significar secções separadas.
1. Em seguida, preencha o texto do corpo utilizando o projeto de material na secção Deinsights do Cliente da página regra da Alquimia
    1. Listas de balas estão bem.
    1. Listas numeradas também
    1. **Arrojado** e *itálico* são um ok
    1. As ligações devem ser sempre **"links para web"/external** OU **deep-links para elementos UI**, e não ligações internas.
    1. As imagens não são oficialmente apoiadas neste momento, mas está no roteiro.

E isto já é um pouco longo demais. A melhor prática é cerca de 400 caracteres ---------------------------------

Assim que o conteúdo estiver pronto, puxe-o para o ramo vivo. Em seguida, vá ao [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) e introduza o nome de ficheiro no campo de url. 