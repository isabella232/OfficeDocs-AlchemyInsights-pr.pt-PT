---
title: Migração sharePoint acelerando com 503 erros
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931669"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="dd4de-102">Migração sharePoint acelerando com 503 erros</span><span class="sxs-lookup"><span data-stu-id="dd4de-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="dd4de-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="dd4de-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="dd4de-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="dd4de-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="dd4de-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="dd4de-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="dd4de-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="dd4de-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="dd4de-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="dd4de-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="dd4de-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="dd4de-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="dd4de-109">**503 erros ao migrar para o SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="dd4de-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="dd4de-110">Parece que está a migrar para o SharePoint Online e a receber 503 erros.</span><span class="sxs-lookup"><span data-stu-id="dd4de-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="dd4de-111">Por favor, siga os passos abaixo para que possamos ajudá-lo o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="dd4de-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="dd4de-112">Clique em Suporte de **Contato,** e, em seguida, **Novo Pedido de Serviço**.</span><span class="sxs-lookup"><span data-stu-id="dd4de-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="dd4de-113">Para o título e descrição, digite o **Throttling de Migração SharePoint com 503**.</span><span class="sxs-lookup"><span data-stu-id="dd4de-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="dd4de-114">Uma vez que o bilhete tenha sido submetido, por favor atualize-o com as seguintes informações:</span><span class="sxs-lookup"><span data-stu-id="dd4de-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="dd4de-115">Quanto resta da migração (por exemplo, quantos TBs?).</span><span class="sxs-lookup"><span data-stu-id="dd4de-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="dd4de-116">Migração início e fim data.</span><span class="sxs-lookup"><span data-stu-id="dd4de-116">Migration start and end date.</span></span>
    - <span data-ttu-id="dd4de-117">Descreva de onde está a migrar o seu conteúdo, como SharePoint Server, Box, GDrive, File shares, etc.</span><span class="sxs-lookup"><span data-stu-id="dd4de-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="dd4de-118">Estimar o número de erros de estrangulamento (por exemplo, x acelerador por hora?) e quando é que o estrangulamento aconteceu.</span><span class="sxs-lookup"><span data-stu-id="dd4de-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="dd4de-119">Que ferramenta de migração está a usar (por exemplo, SPMT ou ShareGate).</span><span class="sxs-lookup"><span data-stu-id="dd4de-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


