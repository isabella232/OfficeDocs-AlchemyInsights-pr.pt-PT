---
title: Estrangulamento online sharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931453"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="a1ac9-102">Estrangulamento online sharePoint</span><span class="sxs-lookup"><span data-stu-id="a1ac9-102">SharePoint Online throttling</span></span>

<span data-ttu-id="a1ac9-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a1ac9-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a1ac9-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a1ac9-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a1ac9-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a1ac9-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a1ac9-109">**Estrangulamento online sharePoint**</span><span class="sxs-lookup"><span data-stu-id="a1ac9-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="a1ac9-110">O SharePoint Online utiliza o estrangulamento para manter o desempenho e a fiabilidade ideais do serviço SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a1ac9-111">O estrangulamento limita o número de ações do utilizador ou chamadas simultâneas (por script ou código) para evitar o uso excessivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="a1ac9-112">Para mais informações, visite os links abaixo.</span><span class="sxs-lookup"><span data-stu-id="a1ac9-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="a1ac9-113">Evite ser estrangulado ou bloqueado no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a1ac9-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="a1ac9-114">Migração de dados e estrangulamento do SPO</span><span class="sxs-lookup"><span data-stu-id="a1ac9-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="a1ac9-115">SharePoint Online e OneDrive Velocidade de migração</span><span class="sxs-lookup"><span data-stu-id="a1ac9-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="a1ac9-116">Manuseie o estrangulamento online do SharePoint através da utilização de back off exponencial</span><span class="sxs-lookup"><span data-stu-id="a1ac9-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="a1ac9-117">Planeamento de capacidade e testes de carga SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a1ac9-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

