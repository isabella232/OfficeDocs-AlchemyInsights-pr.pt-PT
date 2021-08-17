---
title: Os conteúdos não são apresentados nos resultados da pesquisa do SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081621"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Os conteúdos não são apresentados nos resultados da pesquisa do SharePoint

Siga estes passos de remoção de problemas quando os conteúdos esperados não aparecerem nos resultados da pesquisa:
  
1. Verifique se o **site que contém** o conteúdo esperado está definido para permitir que os conteúdos apareçam nos resultados da pesquisa. Siga os passos em [Mostrar conteúdo num site nos resultados da pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verifique se a **lista ou** biblioteca **que contém** o conteúdo esperado está definida para permitir que os conteúdos apareçam nos resultados da pesquisa. Siga os passos em [Mostrar conteúdo de listas ou bibliotecas nos resultados da pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verifique se a página, o documento ou o esquema de página personalizado estão publicados como uma **Versão principal.** Siga o passo 3 [em A Pesquisa não devolve todos os resultados no SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Verifique se o utilizador tem **permissões** para ver os conteúdos. Siga os passos em Compreender [os níveis de permissão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se o esquema de pesquisa tiver sido alterado ao adicionar uma nova propriedade gerida, ao editar uma propriedade gerida ou ao remover uma propriedade gerida, será necessária uma pesquisa e indexação nova. **Indexe o** conteúdo ao seguir os passos em Pedir manualmente a indexação e a indexação de um [site, biblioteca ou lista.](https://docs.microsoft.com/sharepoint/crawl-site-content) Esta ação poderá demorar algum tempo, aguarde 24 horas antes de voltar a verificar os resultados.

Para obter mais informações, consulte [Permitir que o conteúdo num site seja pesculhável.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
