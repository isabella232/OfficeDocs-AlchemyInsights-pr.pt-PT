---
title: o mesmo que o nome de ficheiro é melhor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918906"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Obrigatório Cabeçalho Alquimia H1, H2 não funciona."
Práticas Recomendadas e diretrizes para a autoria alquimia:

1. **Não aninhar Alquimia Informações em pastas –** esta ação irá quebrar a estrutura do URL. Estamos a tentar corrigir isto.
1. Os ficheiros **na pasta AlchemyInsights** devem ter nome de ficheiros em minúsculas com hífens para espaços, por exemplo. **_how-to-enable-litigation-hold_**.
    1. Inclua o ID da Regra ou O ID do grupo do [portal parceiro Alchemy](https://alchemyportal.azurewebsites.net) no campo ms.custom. por ex.: ***ms.custom: 100021***
1. Utilize os restantes metadados na parte superior deste ficheiro como modelo.
1. No [portal parceiro Alchemy,](https://alchemyportal.azurewebsites.net)navegue para baixo até à secção Título da Informação do **Cliente:** e utilize-o como ponto de partida para o seu título H1 para as suas insights. 
    > [!NOTE]
    > A alquimia Informações TEM de ter apenas um H1 na parte superior ou deixará de estar em produção. Os H2 não são apresentados, por isso utilize **negrito** ou outras convenções para significar secções separadas.
1. Em seguida, preencha o corpo de texto com o material de rascunho Informações do Cliente secção da página Regra De Alquimia
    1. As listas com marcas estão bem
    1. Também pode ver listas numeradas
    1. **Negrito** *e itálico* estão a-ok
    1. As ligações devem ser sempre "ligações para a **Web"/ligações externas** OU ligações profundas para elementos da **IU** e não ligações internas.
    1. As imagens não são oficialmente suportadas neste momento, mas estão no caminho certo.

E isto já é um pouco demasiado longo. A melhor prática é cerca de 400 carateres ---------------------------------

Assim que os seus conteúdos estiverem prontos, puxe-os para a filial em tempo real. Em seguida, vá para o [portal parceiro Alchemy](https://alchemyportal.azurewebsites.net) e introduza o nome do ficheiro no campo de URL. 