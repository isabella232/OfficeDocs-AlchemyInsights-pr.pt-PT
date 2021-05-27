---
title: A remoção de problemas de deteção de problemas deteção de erros
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676279"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="084a2-102">A remoção de problemas de deteção de problemas deteção de erros</span><span class="sxs-lookup"><span data-stu-id="084a2-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="084a2-103">Está a ter problemas com as deteções de e-?</span><span class="sxs-lookup"><span data-stu-id="084a2-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="084a2-104">Eis algumas práticas recomendadas a ter em conta:</span><span class="sxs-lookup"><span data-stu-id="084a2-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="084a2-105">Verifique o estado da distribuição em espera.</span><span class="sxs-lookup"><span data-stu-id="084a2-105">Check the hold distribution status.</span></span>  <span data-ttu-id="084a2-106">Se o estado estiver **Atual (Pendente)** ou **Desativado (Pendente),** aguarde até que a distribuição em suspensão seja concluída.</span><span class="sxs-lookup"><span data-stu-id="084a2-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="084a2-107">Intercalie as atualizações da Deteção de Dados Eletrões num único pedido em massa em vez de atualizar a política repetidamente para cada transação.</span><span class="sxs-lookup"><span data-stu-id="084a2-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="084a2-108">Execute Set-CaseHoldPolicy <policyname> -RetryDistribution no PowerShell do Centro de Conformidade e Segurança.</span><span class="sxs-lookup"><span data-stu-id="084a2-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="084a2-109">Para obter detalhes, consulte [Ligação Centro de Conformidade & PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="084a2-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="084a2-110">Para obter os passos para verificar estas definições e práticas recomendadas adicionais para a mitigação e resolução de problemas de Deteção de Dados Técnicos, consulte Resolução de problemas de erros de deteção de [dados técnicos.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="084a2-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="084a2-111">Para mais informações sobre a resolução de outros problemas comuns na Deteção de Dados Online, consulte Investigar, resolver problemas e resolver problemas comuns na Deteção [de Dados Dados Online.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="084a2-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
