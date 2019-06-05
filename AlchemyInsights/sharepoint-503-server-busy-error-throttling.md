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
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716937"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="48045-102">A optimização Online do SharePoint</span><span class="sxs-lookup"><span data-stu-id="48045-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="48045-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Os utilizadores poderão receber um 503 servidor estiver ocupado erro quando tentar navegar para sites Sharepoint ou OneDrive.</span></span><span class="sxs-lookup"><span data-stu-id="48045-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="48045-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Este erro pode ser causado pelo estreitamento dentro do serviço Sharepoint. SharePoint Online utiliza optimização para manter um óptimo desempenho e fiabilidade do serviço Online do SharePoint. Limites de estreitamento o número de acções do utilizador ou em simultâneo chamadas (por script ou código) para impedir a utilização excessiva de recursos. Se é limitada, 99% de tempo deve-se a código personalizado.</span></span><span class="sxs-lookup"><span data-stu-id="48045-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="48045-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Para mais informações sobre optimização <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">evitar obter limitada ou bloqueado no SharePoint Online</a>, consulte.</span></span><span class="sxs-lookup"><span data-stu-id="48045-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="48045-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Se acha que este erro está relacionado com o estreitamento, pode verificar se existe manutenção activa que ocorram no seu tenant navegando para o <a href="https://portal.office.com/adminportal/home#/MessageCenter">Centro de mensagens</a>. Finalmente, certifique-se de que visitar a página de <a href="https://portal.office.com/adminportal/home#/servicehealth">Estado de funcionamento do serviço</a> para verificar a existência de quaisquer avisos/incidentes que pode estar a ocorrer.</span></span><span class="sxs-lookup"><span data-stu-id="48045-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>


