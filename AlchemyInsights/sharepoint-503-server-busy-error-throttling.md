---
title: Limitação on-line sharepoint
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048627"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5e4be-102">Limitação on-line sharepoint</span><span class="sxs-lookup"><span data-stu-id="5e4be-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5e4be-103">Os usuários podem receber um servidor 503 é um erro ocupado ao tentar navegar para sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5e4be-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5e4be-104">Esse erro pode ser causado pela limitação dentro do serviço SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5e4be-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5e4be-105">O SharePoint Online usa a limitação para manter o desempenho ideal e a confiabilidade do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="5e4be-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5e4be-106">A limitação limita o número de ações do usuário ou chamadas simultâneas (por script ou código) para evitar o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="5e4be-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5e4be-107">Se você for estrangulado, 99% do tempo é por causa do código personalizado.</span><span class="sxs-lookup"><span data-stu-id="5e4be-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="5e4be-108">Para obter mais informações sobre a limitação veja, [evite ser estrangulado ou bloqueado no SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="5e4be-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5e4be-109">Se você acredita que este erro não está relacionado à limitação, você pode verificar se há manutenção ativa ocorrendo em seu inquilino navegando para o centro de [mensagens.](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="5e4be-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5e4be-110">Por fim, certifique-se de visitar a página [de Saúde](https://portal.office.com/adminportal/home#/servicehealth) do Serviço para verificar se há avisos/incidentes que possam estar ocorrendo.</span><span class="sxs-lookup"><span data-stu-id="5e4be-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

