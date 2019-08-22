---
title: A optimização Online do SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559852"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="cb383-102">A optimização Online do SharePoint</span><span class="sxs-lookup"><span data-stu-id="cb383-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="cb383-103">Os utilizadores poderão receber um 503 servidor estiver ocupado erro quando tentar navegar para sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cb383-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="cb383-104">Este erro pode ser causado pelo estreitamento dentro do serviço SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cb383-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="cb383-105">SharePoint Online utiliza optimização para manter um óptimo desempenho e fiabilidade do serviço Online do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cb383-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="cb383-106">Limites de estreitamento o número de acções do utilizador ou em simultâneo chamadas (por script ou código) para impedir a utilização excessiva de recursos.</span><span class="sxs-lookup"><span data-stu-id="cb383-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="cb383-107">Se é limitada, 99% de tempo deve-se a código personalizado.</span><span class="sxs-lookup"><span data-stu-id="cb383-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="cb383-108">Para mais informações sobre optimização [evitar obter limitada ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online), consulte.</span><span class="sxs-lookup"><span data-stu-id="cb383-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="cb383-109">Se acha que este erro está relacionado com o estreitamento, pode verificar se existe manutenção activa que ocorram no seu tenant navegando para o [Centro de mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="cb383-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="cb383-110">Finalmente, certifique-se de que visitar a página de [Estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth) para verificar a existência de quaisquer avisos/incidentes que pode estar a ocorrer.</span><span class="sxs-lookup"><span data-stu-id="cb383-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

