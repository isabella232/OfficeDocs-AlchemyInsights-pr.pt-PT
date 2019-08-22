---
title: Conteúdo não aparece nos resultados da pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517042"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Conteúdo não aparece nos resultados da pesquisa do SharePoint

Siga estes passos de resolução de problemas quando conteúdo esperado não aparece nos resultados da procura:
  
1. Verifique se o **site** que contém o conteúdo esperado está definidas para permitir a apresentação nos resultados da pesquisa de conteúdo. Siga os passos de [Mostrar conteúdo num site nos resultados da procura](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verifique que a **lista** ou **biblioteca** que contém o conteúdo esperado está definido para permitir a apresentação nos resultados da pesquisa de conteúdo. Siga os passos de [Mostrar o conteúdo das listas ou bibliotecas nos resultados da procura](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Certifique-se de que a página, documento ou esquema de página personalizada é publicada como uma **versão principal.** Siga o passo 3 na [procura não devolver todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Certifique-se de que o utilizador tem **permissões** para ver o conteúdo. Siga os passos nos [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se o esquema de pesquisa foi alterado adicionando uma nova propriedade gerida, através da edição de uma propriedade gerida ou removendo uma propriedade gerida, em seguida, pedir uma pesquisa e re-indexar será necessário. **Re-indexar** o conteúdo seguindo os passos no [pedido manualmente de pesquisa e indexação voltar de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Isto poderá demorar alguns minutos, aguarde 24 horas antes de verificar os resultados novamente.

Para mais informações, consulte [Activar o conteúdo de um site para ser procurado](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
