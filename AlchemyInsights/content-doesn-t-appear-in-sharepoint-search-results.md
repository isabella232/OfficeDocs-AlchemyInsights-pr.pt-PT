---
title: O conteúdo não aparece nos resultados de pesquisa do SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713141"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>O conteúdo não aparece nos resultados de pesquisa do SharePoint

Siga estes passos de resolução de problemas quando o conteúdo esperado não aparece nos resultados da pesquisa:
  
1. Verifique se o **site** que contém o conteúdo esperado está definido para permitir que o conteúdo apareça nos resultados da pesquisa. Siga os passos em [Mostrar conteúdo num site em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verifique se a **lista** ou **biblioteca** que contém o conteúdo esperado está definida para permitir que o conteúdo apareça nos resultados da pesquisa. Siga os passos em [Mostrar conteúdo de listas ou bibliotecas em resultados de pesquisa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verifique se a página, documento ou layout de página personalizada é publicado como uma **versão Major.** Siga o passo 3 na [Search não devolva todos os resultados no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verifique se o utilizador tem **permissões** para visualizar o conteúdo. Siga os passos nos [níveis de permissão de compreensão no SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Se o esquema de pesquisa tiver sido alterado adicionando uma nova propriedade gerida, editando uma propriedade gerida, ou removendo uma propriedade gerida, então solicitar um rastreio e re-indexamento será necessário. **Re-indexar** o conteúdo seguindo os passos em [Manualmente solicitar o rastreio e re-indexação de um site, uma biblioteca ou uma lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Isto pode demorar um pouco, esperar 24 horas antes de verificar os resultados novamente.

Para obter mais informações, consulte [Ativar o conteúdo de um site a pes pes que possa ser pes pes pesável.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
