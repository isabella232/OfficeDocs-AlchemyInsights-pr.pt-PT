---
title: 'mesmo que o nome de ficheiro é melhor [regra #-descrição]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634515"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Necessário Alquimia cabeçalho H1, H2 não funcionam.
Procedimentos recomendados e orientações para a criação de Alquimia:

1. **Não se aninham conhecimentos aprofundados de Alquimia em pastas**- Isto irá interromper a estrutura de URLs. Procuramos, para corrigir isto.
1. Ficheiros na pasta **AlchemyInsights** devem ter o ID da regra e o nome da regra a partir do [portal para parceiros de Alquimia](https://alchemyportal.azurewebsites.net) no nome de ficheiro.
    1. ex. ***976-How-to-Enable-litigation-Hold***
1. Utilize os metadados na parte superior deste ficheiro como modelo. Nada mais é necessário.
1. No [portal para parceiros de Alquimia](https://alchemyportal.azurewebsites.net), navegue para a secção **cliente Insight título:** e a utilização que, como um iniciar, aponte para o título H1 para a visão. 
    > [!NOTE]
    > Alquimia informações privilegiadas deve ter apenas um único H1 na parte superior ou vão quebrar na produção. H2s não compor assim utilização **negrito** ou outras convenções para significar secções separadas.
1. Em seguida, preencha o corpo de texto utilizando o material de projecto na secção informações de cliente da página regra de Alquimia
    1. Listas com marcas estão correctos
    1. Listas numeradas demasiado
    1. **Negrito** e *itálico* são a-ok
    1. Hiperligações devem ser sempre quer **"ligações Web" / externo** ou **deep-hiperligações para elementos da IU**, as hiperligações não internas.

E realmente já é um pouco demasiado longo. Recomenda-se cerca de 400 caracteres--

Depois do conteúdo estiver pronto, puxe-lo para o ramo vivo. Em seguida, vá para o [portal de parceiro de Alquimia](https://alchemyportal.azurewebsites.net) e introduza o nome de ficheiro para o campo de url. Certifique-se de conhecimentos aprofundados revistas e publicadas indicar "Sim" e, em seguida, faça clique sobre a regra de actualização. **(Esta procura prettier na nova versão do portal - logo que a libertação.)** 
 ![campo url](media/for-content-team.PNG)

