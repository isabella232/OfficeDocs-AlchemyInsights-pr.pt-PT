---
title: mesmo que o nome de arquivo é melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800056"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obrigado Alquimia Cabeçalho H1, H2 não funcionam.
Melhores práticas e diretrizes para a autoria da Alquimia:

1. **Não aninhe Alchemy Insights em pastas**- isso vai quebrar a estrutura url. Estamos procurando consertar isso.
1. Arquivos na pasta **AlchemyInsights** devem ter nomes de arquivos minúsculos com hífens para espaços ex. ***como habilitar-litígio-hold***.
    1. Inclua a identificação da régua ou a identificação do balde do portal do sócio da [alquimia](https://alchemyportal.azurewebsites.net) no campo do ms.custom. Ex. ***ms.custom: 100021 ms.custom: 100021***
1. Use o resto dos metadados na parte superior deste arquivo como modelo.
1. No [portal Alchemy Partner,](https://alchemyportal.azurewebsites.net)navegue até a seção Título de Percepção do **Cliente:** e use isso como ponto de partida para o seu título H1 para obter informações. 
    > [!NOTE]
    > Alquimia Insights deve ter apenas um único H1 no topo ou eles vão quebrar na produção. Os H2s não tornam o **uso ousado** ou outras convenções para significar seções separadas.
1. Em seguida, preencha o texto do corpo usando o material de rascunho na seção Insights do Cliente da página regra de alquimia
    1. Listas bulleted são muito bem
    1. Listas numeradas também
    1. **Negrito** e *itálico* são a-ok
    1. Links devem ser sempre **"links para web" / externa** ou **links profundos para elementos**de ura, não links internos.
    1. As imagens não são oficialmente suportadas neste momento, mas está no roteiro.

E isso já é realmente um pouco longo demais. A melhor prática é de cerca de 400 personagens ---------------------------------

Uma vez que seu conteúdo está pronto, puxá-lo para o ramo ao vivo. Em seguida, vá para o [portal Alchemy Partner](https://alchemyportal.azurewebsites.net) e digite o nome de arquivo no campo url. 