---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068424"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

O SharePoint ou o OneDrive podem ser lentos, inacessíveis ou indisponíveis ou podem exibir um serviço indisponível ou 503 erros, por várias razões:
  
- Se o site SharePoint ou OneDrive estiver lento ou atrasado para vários usuários, pode haver um problema de serviço temporário em que os usuários experimentam atrasos intermitentes ou erros de navegação ao acessar sites do SharePoint ou conteúdo do OneDrive. Verifique o painel de saúde do [Serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização está afetada.
  
- Os usuários podem receber um *servidor 503 é* um erro ocupado ao tentar navegar para sites SharePoint ou OneDrive. Esse erro pode ser causado pela limitação dentro do serviço SharePoint. O SharePoint Online usa a limitação para manter o desempenho ideal e a confiabilidade do serviço SharePoint Online. A limitação limita o número de ações do usuário ou chamadas simultâneas (por script ou código) para evitar o uso excessivo de recursos. Para obter mais informações sobre a limitação veja, [evite ser estrangulado ou bloqueado no SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Se você experimentar um desempenho lento com um site ou página **clássico** ou **moderno** do SharePoint, utilize a ferramenta [Page Diagnostic](https://aka.ms/perftool) para analisar as páginas.
  
- Se você ainda experimentar o desempenho lento geral, consulte os recursos na parte inferior deste artigo: Introdução ao ajuste de [desempenho para SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  