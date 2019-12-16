---
title: Pesquisa no SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044054"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Rastreamento de conteúdo e indexação no SharePoint Online

O conteúdo deve ser rastreado e adicionado ao índice de pesquisa para que os usuários encontrem o que estão pesquisando no SharePoint Online. O conteúdo é automaticamente rastreado com base em um cronograma de rastreamento pré-definido (o cronograma de rastreamento não pode ser alterado). O rastreador capta conteúdo que mudou desde o último rastreamento e atualiza o índice. Para garantir que o conteúdo seja rastreado e o índice seja atualizado, observe o seguinte:

- Certifique-se de que o conteúdo pode ser encontrado tornando o conteúdo do [site pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Quando você mudou uma propriedade controlada, ou quando você mudou o mapeamento de propriedades rastejadas e controladas, o local deve ser re-rastejado antes que suas mudanças sejam refletidas no índice da busca. 

    Como suas alterações são feitas no esquema de pesquisa e não no site real, o rastreador não reindexará automaticamente o site. 

    Para mais informações, consulte [manualmente rastreamento e re-indexação de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Espere pelo menos 24 horas depois de solicitar manualmente um rastreamento e re-índice completo para ver se você ainda está enfrentando um problema. 

    Se mais de 24 horas se passaram desde que você iniciou o rastreamento e re-índice completo, por favor, registre um caso de suporte. Em muitos casos, já estamos trabalhando em uma solução. Por favor, dê-nos pelo menos 24 horas para completar uma solução.

> [!IMPORTANT]
> Se um site, documento (biblioteca) ou uma lista for excluído e ainda for exibido nos resultados da pesquisa, os usuários devem receber um **arquivo Erro 404 não encontrado** ao tentar acessá-lo. Esta questão deve ser registrada como um caso de apoio para uma investigação mais aprofundada. 



