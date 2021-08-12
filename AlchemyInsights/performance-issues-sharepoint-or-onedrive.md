---
title: Problemas de desempenho no SharePoint ou OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911853"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para múltiplos utilizadores

O SharePoint OneDrive pode estar lento, inacessível ou indisponível ou apresentar erros de serviço indisponíveis ou 503, por diversas razões:
  
- Se o seu site do SharePoint ou do OneDrive estiver lento ou atrasado para vários utilizadores, poderá haver um problema de serviço temporário em que os utilizadores se detetam atrasos intermitentes ou erros de navegação ao aceder a sites do SharePoint ou OneDrive conteúdo. Consulte o [dashboard Estado de saúde do](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) serviço para ver se a sua organização é afetada.
  
- Os utilizadores poderão receber um erro de *503* servidores que estão ocupados ao tentarem navegar para o SharePoint ou para OneDrive sites. Este erro pode ser causado pela throttling no serviço SharePoint. O SharePoint Online utiliza a limitação para manter o desempenho e a fiabilidade ideais do serviço do SharePoint Online. A limitação restringe o número de ações do utilizador ou chamadas em simultâneo (por script ou código) para evitar a utilização excessiva de recursos. Para obter mais informações sobre a throttling, consulte Evitar ser retido [ou bloqueado no SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Se o desempenho for lento num site ou página do **SharePoint** clássico ou moderno, utilize **a** ferramenta Diagnóstico de [Página](https://aka.ms/perftool) para analisar as páginas.
  
- Se continuar a experienciar um desempenho lento geral, reveja os recursos na parte inferior deste artigo: Introdução à ofinação do [desempenho do SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  