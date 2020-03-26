---
title: Desempenho da migração do SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932245"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="6a4a2-102">Desempenho da migração do SharePoint</span><span class="sxs-lookup"><span data-stu-id="6a4a2-102">SharePoint migration performance</span></span>

<span data-ttu-id="6a4a2-103">**Importante**: muitos clientes do SharePoint Online e OneDrive executam aplicações essenciais para as empresas no serviço que são executadas em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6a4a2-104">Estas incluem soluções de migração de conteúdos, Prevenção de Perda de Dados (DLP) de cópia de segurança.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6a4a2-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho à distância.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6a4a2-106">Como medida de suporte a este objetivo, implementámos limitações mais restritas em aplicações de segundo plano (soluções de migração, DLP e cópias de segurança) durante as horas diurnas dos dias úteis.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6a4a2-107">Deverá esperar uma limitação bastante restrita por parte destas aplicações durante este período de tempo.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6a4a2-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6a4a2-109">**Desempenho da migração**</span><span class="sxs-lookup"><span data-stu-id="6a4a2-109">**Migration performance**</span></span>

<span data-ttu-id="6a4a2-110">O desempenho da migração pode ser afetado pela infraestrutura da rede, tamanho dos ficheiros, tempo de migração e limitações.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="6a4a2-111">Compreender estes fatores vai ajudá-lo a planear e maximizar a eficácia da sua migração.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="6a4a2-112">Para obter mais informações, visite as ligações abaixo.</span><span class="sxs-lookup"><span data-stu-id="6a4a2-112">For more information, please visit the links below.</span></span>

- <span data-ttu-id="6a4a2-113">[Sharepoint Online and ODB Migration Speed](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed) (Velocidade da Migração do SharePoint Online e do ODB)</span><span class="sxs-lookup"><span data-stu-id="6a4a2-113">[Sharepoint Online and ODB Migration Speed](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)</span></span>

- <span data-ttu-id="6a4a2-114">[Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online) (Evitar ser limitado ou bloqueado no SharePoint Online)</span><span class="sxs-lookup"><span data-stu-id="6a4a2-114">[Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span></span>

- <span data-ttu-id="6a4a2-115">[Download and install the SharePoint Migration Tool](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool) (Transferir e Instalar a Ferramenta de Migração do SharePoint)</span><span class="sxs-lookup"><span data-stu-id="6a4a2-115">[Download and install the SharePoint Migration Tool](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)</span></span>
