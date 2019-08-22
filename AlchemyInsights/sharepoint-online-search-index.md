---
title: Procurar no SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507642"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Conteúdo de pesquisa e indexação no SharePoint Online

Conteúdo deve ser pesquisado e adicionado ao índice de procura aos utilizadores a localização daquilo procura no SharePoint Online. Conteúdo é pesquisado automaticamente com base numa agenda de pesquisa predefinido (não é possível alterar a agenda de pesquisa). O crawler capta conteúdo que foi alterado desde a última pesquisa e actualiza o índice. Para garantir o conteúdo é pesquisado e o índice é actualizado, tenha em atenção o seguinte:

- Certifique-se de conteúdo pode ser encontrado, [tornando o conteúdo do site pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Quando alterar uma propriedade gerida ou quando alterou o mapeamento de pesquisado e geridos propriedades, o site tem de ser novamente pesquisadas antes das alterações serão reflectidas no índice de pesquisa. 

    Uma vez que as alterações serão efectuadas no esquema de procura e não para o site actual, o crawler não adicionará automaticamente re-indexe o site. 

    Para obter mais informações, consulte [Pedir manualmente de pesquisa e indexação voltar de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Aguarde, pelo menos, 24 horas após solicitar manualmente uma pesquisa e, em seguida, completa reindexar para ver se ainda estiver com um problema. 

    Se tiverem passado mais de 24 horas desde que iniciou a pesquisa e, em seguida, reindexar completo, inicie a sessão de um incidente de suporte. Em muitos casos, a Microsoft já estiver a trabalhar numa solução. Forneça pelo menos 24 horas para concluir uma solução.

> [!IMPORTANT]
> Se um site, uma lista ou documento (biblioteca) foi eliminado e continua a aparecer nos resultados da procura, os utilizadores devem receber um **Erro 404 ficheiro não encontrado** ao tentar aceder a ele. Este problema deve ser registado como um incidente de suporte para a investigação suplementar. 



