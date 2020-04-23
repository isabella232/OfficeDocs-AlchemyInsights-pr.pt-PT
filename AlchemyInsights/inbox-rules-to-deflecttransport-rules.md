---
title: 929 Regras de caixa de entrada para desviar regras de transporte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724603"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="3ba56-102">Regras de fluxo de correio (também conhecidas como regras de transporte)</span><span class="sxs-lookup"><span data-stu-id="3ba56-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="3ba56-103">Visão geral das regras de fluxo de correio: Regras de fluxo de [correio (regras de transporte) em Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="3ba56-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="3ba56-104">Regras de fluxo de correio de configuração: [Procedimentos](https://technet.microsoft.com/library/dn600436.aspx) de regra de fluxo de correio em Exchange Online</span><span class="sxs-lookup"><span data-stu-id="3ba56-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="3ba56-105">Criar, modificar e eliminar regras de fluxo de correio: [Gerir as regras](https://technet.microsoft.com/library/jj657505.aspx) de fluxo de correio</span><span class="sxs-lookup"><span data-stu-id="3ba56-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="3ba56-106">Também pode gerir as regras de fluxo de correio em Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3ba56-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="3ba56-107">Para mais informações, consulte [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (visualização), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (criar), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (eliminar), [Definição de Transporte (modificar](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) existente), Regra de Transporte de [Saem](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (desativação existente) e [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (ativação existente).</span><span class="sxs-lookup"><span data-stu-id="3ba56-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="3ba56-108">Regra adicional de fluxo de correio cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (lista de ações disponíveis), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (lista de condições e exceções disponíveis), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (regras de exportação) e [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (regras de importação).</span><span class="sxs-lookup"><span data-stu-id="3ba56-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
