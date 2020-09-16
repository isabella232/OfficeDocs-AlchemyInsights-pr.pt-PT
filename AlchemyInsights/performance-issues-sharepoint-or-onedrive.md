---
title: Questões de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771912"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lentos, inacessíveis ou indisponíveis para vários utilizadores

O SharePoint ou o OneDrive podem ser lentos, inacessíveis ou indisponíveis, ou podem apresentar o serviço indisponível ou 503 erros, por várias razões:
  
- Se o seu site SharePoint ou OneDrive for lento ou atrasado para vários utilizadores, pode haver um problema de serviço temporário onde os utilizadores experimentam atrasos intermitentes ou erros de navegação ao aceder a sites SharePoint ou conteúdo OneDrive. Consulte o [painel de saúde do Serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se a sua organização está com impacto.
  
- Os utilizadores podem receber um *servidor 503 está a um* erro ocupado ao tentar navegar para sites SharePoint ou OneDrive. Este erro pode ser causado por estrangulamento dentro do serviço SharePoint. O SharePoint Online utiliza a limitação para manter o desempenho e a fiabilidade ideais do serviço do SharePoint Online. A limitação restringe o número de ações do utilizador ou chamadas em simultâneo (por script ou código) para evitar a utilização excessiva de recursos. Para obter mais informações sobre o estrangulamento, [evite ser estrangulado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Se experimentar um desempenho lento com um site ou página do SharePoint **clássico** ou **moderno,** utilize a [ferramenta de Diagnóstico](https://aka.ms/perftool) de Página para analisar as páginas.
  
- Se ainda experimentar um desempenho lento geral, por favor reveja os recursos na parte inferior deste artigo: [Introdução à afinação](https://go.microsoft.com/fwlink/?linkid=2024334) de desempenho para o SharePoint Online
  