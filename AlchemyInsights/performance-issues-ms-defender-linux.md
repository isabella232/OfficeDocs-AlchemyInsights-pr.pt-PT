---
title: Problemas de desempenho do Microsoft Defender para Ponto Final no Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794001"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="40835-102">Problemas de desempenho do Microsoft Defender para Ponto Final no Linux</span><span class="sxs-lookup"><span data-stu-id="40835-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="40835-103">Este artigo guia-o ao longo dos passos de identificação de problemas de desempenho do Microsoft Defender para Endpoint no Linux.</span><span class="sxs-lookup"><span data-stu-id="40835-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="40835-104">Primeiro, é importante verificar se o problema que está a ter foi resolvido com a versão [mais recente.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="40835-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="40835-105">Para iniciar a sua investigação, consulte [Remoção de problemas de desempenho do Microsoft Defender para Endpoint no Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="40835-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="40835-106">Exclusões</span><span class="sxs-lookup"><span data-stu-id="40835-106">Exclusions</span></span>

<span data-ttu-id="40835-107">As exclusões podem ajudar a mitigar problemas de desempenho.</span><span class="sxs-lookup"><span data-stu-id="40835-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="40835-108">Reveja as suas exclusões antes de começar para que qualquer risco adicional seja conhecido e documentado.</span><span class="sxs-lookup"><span data-stu-id="40835-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="40835-109">Para obter mais informações, consulte [Configurar e validar exclusões do Microsoft Defender para Pontos Finais no Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="40835-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="40835-110">Quando tiver múltiplos ficheiros & pastas a excluir e se encontrarem todos no mesmo ponto de montagem, poderá ser mais fácil excluir o ponto de montagem.</span><span class="sxs-lookup"><span data-stu-id="40835-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="40835-111">A partir do lançamento de fevereiro 101.22.80, pode excluir uma montagem inteira.</span><span class="sxs-lookup"><span data-stu-id="40835-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="40835-112">Por exemplo, se /mnt/backup for um ponto de montagem, pode adicionar /mnt/backup à lista de exclusões ao executar este comando:</span><span class="sxs-lookup"><span data-stu-id="40835-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="40835-113">**Nota:** adicionar exclusões aumenta o risco de o software malicado não ser detetado e deve ser tratado e implementado com cuidado.</span><span class="sxs-lookup"><span data-stu-id="40835-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="40835-114">Precisa de Ajuda?</span><span class="sxs-lookup"><span data-stu-id="40835-114">Need Help?</span></span>

<span data-ttu-id="40835-115">Para o ajudar da forma mais eficiente, recolha os dados de diagnóstico antes de abrir um caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="40835-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
