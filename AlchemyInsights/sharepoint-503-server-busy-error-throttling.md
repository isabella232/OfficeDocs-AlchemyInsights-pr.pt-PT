---
title: SharePoint Online Throttling
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773858"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="7e6c7-102">SharePoint Online Throttling</span><span class="sxs-lookup"><span data-stu-id="7e6c7-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="7e6c7-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="7e6c7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="7e6c7-104">**O servidor 503 está ocupado erro**</span><span class="sxs-lookup"><span data-stu-id="7e6c7-104">**503 server is busy error**</span></span>

<span data-ttu-id="7e6c7-105">Os utilizadores podem receber um servidor 503 está a um erro ocupado ao tentar navegar para sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7e6c7-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="7e6c7-106">Este erro pode ser causado por estrangulamento dentro do serviço SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e6c7-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="7e6c7-107">O SharePoint Online utiliza a limitação para manter o desempenho e a fiabilidade ideais do serviço do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7e6c7-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="7e6c7-108">A limitação restringe o número de ações do utilizador ou chamadas em simultâneo (por script ou código) para evitar a utilização excessiva de recursos.</span><span class="sxs-lookup"><span data-stu-id="7e6c7-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="7e6c7-109">Para obter mais informações sobre o estrangulamento, [evite ser estrangulado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="7e6c7-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="7e6c7-110">Se acredita que este erro não está relacionado com o estrangulamento, pode verificar se existe manutenção ativa no seu inquilino navegando para o [Centro de Mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="7e6c7-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="7e6c7-111">Por fim, certifique-se de que visita a página [de Saúde](https://portal.office.com/adminportal/home#/servicehealth) do Serviço para verificar quaisquer avisos/incidentes que possam ocorrer.</span><span class="sxs-lookup"><span data-stu-id="7e6c7-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

