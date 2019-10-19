---
title: mesmo que o nome do arquivo é melhor
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800056"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Cabeçalho de alquimia obrigatório H1, H2's não funciona.
Melhores práticas e diretrizes para criação de alquimia:

1. **Não aninhar o Alchemy insights em pastas**-isso quebrará a estrutura de URL. Estamos procurando consertar isso.
1. Os arquivos na pasta **Alchemyinsights** devem ter nomes de arquivo minúsculos com hífens para espaços ex. ***How-to-Enable-litígio-Hold***.
    1. Inclua o ID da regra ou o ID do Bucket no [portal do parceiro de alquimia](https://alchemyportal.azurewebsites.net) no campo MS. Custom. Ex. ***MS. Custom: 100021***
1. Use o restante dos metadados na parte superior deste arquivo como seu modelo.
1. No [portal do parceiro de alquimia](https://alchemyportal.azurewebsites.net), navegue até a seção **título do cliente Insight:** e use isso como um ponto de partida para o seu título H1 para o Insight. 
    > [!NOTE]
    > O Alchemy insights deve ter apenas um único H1 na parte superior ou eles quebrarão na produção. O H2S não renderiza tanto o uso de convenções **Bold** ou Other para significar seções separadas.
1. Em seguida, preencha o texto do corpo usando o material de rascunho na seção insights do cliente da página regra de alquimia
    1. Listas com marcadores estão bem
    1. Listas numeradas também
    1. **Negrito** e *itálico* são a-ok
    1. Links devem ser sempre **"links para Web"/External** ou **Deep-links para elementos de interface do usuário**, não links internos.
    1. As imagens não são oficialmente suportadas neste momento, mas é sobre o roteiro.

E isso já é um pouco longo demais. A melhor prática é de cerca de 400 caracteres---------------------------------

Quando o conteúdo estiver pronto, puxe-o para a ramificação ao vivo. Em seguida, vá para o [portal do parceiro de alquimia](https://alchemyportal.azurewebsites.net) e insira o nome do arquivo no campo URL. 