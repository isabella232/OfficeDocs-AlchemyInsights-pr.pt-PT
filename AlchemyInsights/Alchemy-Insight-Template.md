---
title: igual ao nome de ficheiro é melhor
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
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786424"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Necessário Alquimia cabeçalho H1, H2 não funcionam.
Procedimentos recomendados e orientações para a criação de Alquimia:

1. **Não se aninham conhecimentos aprofundados de Alquimia em pastas**- Isto irá interromper a estrutura de URLs. Procuramos, para corrigir isto.
1. Ficheiros na pasta **AlchemyInsights** devem ter nomes de ficheiros em minúsculas com hífenes para espaços ex. ***how-para-activar-litígio-aguardar***.
    1. Inclua o ID de ID da regra ou balde a partir do [portal para parceiros de Alquimia](https://alchemyportal.azurewebsites.net) no campo ms.custom. ex. ***MS.Custom: 100021***
1. Utilize o resto dos metadados na parte superior deste ficheiro como modelo.
1. No [portal para parceiros de Alquimia](https://alchemyportal.azurewebsites.net), navegue para a secção **cliente Insight título:** e a utilização que, como um iniciar, aponte para o título H1 para a visão. 
    > [!NOTE]
    > Alquimia informações privilegiadas deve ter apenas um único H1 na parte superior ou vão quebrar na produção. H2s não compor assim utilização **negrito** ou outras convenções para significar secções separadas.
1. Em seguida, preencha o corpo de texto utilizando o material de projecto na secção informações de cliente da página regra de Alquimia
    1. Listas com marcas estão correctos
    1. Listas numeradas demasiado
    1. **Negrito** e *itálico* são a-ok
    1. Hiperligações devem ser sempre quer **"ligações Web" / externo** ou **deep-hiperligações para elementos da IU**, as hiperligações não internas.
    1. Imagens não são suportadas oficialmente neste momento, mas é o plano.

E realmente já é um pouco demasiado longo. Recomenda-se cerca de 400 caracteres--

Depois do conteúdo estiver pronto, puxe-lo para o ramo vivo. Em seguida, vá para o [portal de parceiro de Alquimia](https://alchemyportal.azurewebsites.net) e introduza o nome de ficheiro para o campo de url. 


