---
title: Diretrizes gerais sobre o desempenho de migrações
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932489"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="e991a-102">Diretrizes gerais sobre o desempenho de migrações</span><span class="sxs-lookup"><span data-stu-id="e991a-102">General migration performance guidance</span></span>

<span data-ttu-id="e991a-103">**Importante**: muitos clientes do SharePoint Online e OneDrive executam aplicações essenciais para as empresas no serviço que são executadas em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="e991a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e991a-104">Estas incluem soluções de migração de conteúdos, Prevenção de Perda de Dados (DLP) de cópia de segurança.</span><span class="sxs-lookup"><span data-stu-id="e991a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e991a-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho à distância.</span><span class="sxs-lookup"><span data-stu-id="e991a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e991a-106">Como medida de suporte a este objetivo, implementámos limitações mais restritas em aplicações de segundo plano (soluções de migração, DLP e cópias de segurança) durante as horas diurnas dos dias úteis.</span><span class="sxs-lookup"><span data-stu-id="e991a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e991a-107">Deverá esperar uma limitação bastante restrita por parte destas aplicações durante este período de tempo.</span><span class="sxs-lookup"><span data-stu-id="e991a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e991a-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="e991a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e991a-109">**Diretrizes sobre o desempenho de migrações**</span><span class="sxs-lookup"><span data-stu-id="e991a-109">**Migration performance guidance**</span></span>

<span data-ttu-id="e991a-110">O desempenho da migração pode ser afetado pela infraestrutura da rede, tamanho dos ficheiros, tempo de migração e limitações.</span><span class="sxs-lookup"><span data-stu-id="e991a-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="e991a-111">Compreender estes fatores vai ajudá-lo a planear e maximizar a eficácia da sua migração.</span><span class="sxs-lookup"><span data-stu-id="e991a-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="e991a-112">Diretrizes gerais sobre o desempenho de migrações</span><span class="sxs-lookup"><span data-stu-id="e991a-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
