---
title: Conteúdo não aparece nos resultados de pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705672"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Conteúdo não aparece nos resultados de pesquisa do SharePoint

Siga estes passos de resolução de problemas quando o conteúdo esperado não aparece nos resultados da pesquisa:
  
1. Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa. Siga os passos em [Mostrar conteúdo num site em resultados](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)de pesquisa .

2. Verifique se a **lista** ou **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa. Siga os passos em [Mostrar conteúdo de listas ou bibliotecas em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verifique se a página, documento ou layout de página personalizado é publicado como uma **versão Major.** Siga o passo 3 em [Search não devolve todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verifique se o utilizador tem **permissões** para visualizar o conteúdo. Siga os passos em compreender os níveis de [permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerida, editando uma propriedade gerida, ou removendo uma propriedade gerida, então será necessário solicitar um rastreio e um re-indexante. **Reindexe** o conteúdo seguindo os passos em [manualmente solicitar rastejar e reindexar um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Isto pode demorar um pouco, espere 24 horas antes de verificar novamente os resultados.

Para mais informações, consulte [Ativar o conteúdo num site para ser pesquisável](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
