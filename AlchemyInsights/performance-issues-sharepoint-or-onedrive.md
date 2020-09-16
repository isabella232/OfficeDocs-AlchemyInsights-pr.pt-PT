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
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="6521a-102">SharePoint ou OneDrive lentos, inacessíveis ou indisponíveis para vários utilizadores</span><span class="sxs-lookup"><span data-stu-id="6521a-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="6521a-103">O SharePoint ou o OneDrive podem ser lentos, inacessíveis ou indisponíveis, ou podem apresentar o serviço indisponível ou 503 erros, por várias razões:</span><span class="sxs-lookup"><span data-stu-id="6521a-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="6521a-104">Se o seu site SharePoint ou OneDrive for lento ou atrasado para vários utilizadores, pode haver um problema de serviço temporário onde os utilizadores experimentam atrasos intermitentes ou erros de navegação ao aceder a sites SharePoint ou conteúdo OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6521a-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="6521a-105">Consulte o [painel de saúde do Serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se a sua organização está com impacto.</span><span class="sxs-lookup"><span data-stu-id="6521a-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="6521a-106">Os utilizadores podem receber um *servidor 503 está a um* erro ocupado ao tentar navegar para sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6521a-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="6521a-107">Este erro pode ser causado por estrangulamento dentro do serviço SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6521a-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6521a-108">O SharePoint Online utiliza a limitação para manter o desempenho e a fiabilidade ideais do serviço do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6521a-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6521a-109">A limitação restringe o número de ações do utilizador ou chamadas em simultâneo (por script ou código) para evitar a utilização excessiva de recursos.</span><span class="sxs-lookup"><span data-stu-id="6521a-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="6521a-110">Para obter mais informações sobre o estrangulamento, [evite ser estrangulado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="6521a-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="6521a-111">Se experimentar um desempenho lento com um site ou página do SharePoint **clássico** ou **moderno,** utilize a [ferramenta de Diagnóstico](https://aka.ms/perftool) de Página para analisar as páginas.</span><span class="sxs-lookup"><span data-stu-id="6521a-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="6521a-112">Se ainda experimentar um desempenho lento geral, por favor reveja os recursos na parte inferior deste artigo: [Introdução à afinação](https://go.microsoft.com/fwlink/?linkid=2024334) de desempenho para o SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6521a-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  