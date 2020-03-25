---
title: SharePoint Online Throttling
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931237"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="9a89d-102">SharePoint Online Throttling</span><span class="sxs-lookup"><span data-stu-id="9a89d-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="9a89d-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="9a89d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9a89d-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="9a89d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9a89d-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="9a89d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9a89d-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="9a89d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9a89d-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="9a89d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9a89d-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="9a89d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9a89d-109">**Servidor 503 está um erro ocupado**</span><span class="sxs-lookup"><span data-stu-id="9a89d-109">**503 server is busy error**</span></span>

<span data-ttu-id="9a89d-110">Os utilizadores podem receber um servidor 503 está um erro de trabalho quando tentam navegar para sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a89d-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="9a89d-111">Este erro pode ser causado por estrangulamento dentro do serviço SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9a89d-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9a89d-112">O SharePoint Online utiliza o estrangulamento para manter o desempenho e a fiabilidade ideais do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9a89d-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9a89d-113">O estrangulamento limita o número de ações do utilizador ou chamadas simultâneas (por script ou código) para evitar o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9a89d-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="9a89d-114">Para obter mais informações sobre o estrangulamento, [evite ser estrangulado ou bloqueado no SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="9a89d-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="9a89d-115">Se você acredita que este erro não está relacionado com estrangulamento, você pode verificar se há manutenção ativa ocorrendo no seu inquilino navegando para o centro de [mensagens](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="9a89d-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="9a89d-116">Por fim, certifique-se de que visita a página [de Saúde](https://portal.office.com/adminportal/home#/servicehealth) de Serviço para verificar se podem ocorrer quaisquer avisos/incidentes.</span><span class="sxs-lookup"><span data-stu-id="9a89d-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

