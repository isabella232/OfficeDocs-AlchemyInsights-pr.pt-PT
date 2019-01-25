---
title: 929 regras de pasta a receber para regras de deflectTransport
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: ed4afe938b310f1569061ad00bf90ad87e91b465
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483821"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="b34aa-102">Regras de fluxo de correio (também conhecido como regras de transporte)</span><span class="sxs-lookup"><span data-stu-id="b34aa-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="b34aa-103">Descrição geral das regras de fluxo de correio: [correio fluxo regras (regras de transporte) no Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="b34aa-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>
    
- <span data-ttu-id="b34aa-104">Regras de fluxo de correio do programa de configuração: [correio fluxo procedimentos de regra no Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="b34aa-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>
    
- <span data-ttu-id="b34aa-105">Criar, modificar e eliminar regras de fluxo de correio: [Gerir regras de fluxo de correio](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="b34aa-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>
    
<span data-ttu-id="b34aa-p101">Também pode gerir regras de fluxo de correio no Exchange Online PowerShell. Para mais informações, consulte [Obter TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (vista), [TransportRule de novo](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (criar), [TransportRule remover](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (eliminar), [Conjunto de TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modificar existente), [TransportRule-desactivar](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existente), e [Activar TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (Active existentes).</span><span class="sxs-lookup"><span data-stu-id="b34aa-p101">You can also manage mail flow rules in Exchange Online PowerShell. For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span> 
  
<span data-ttu-id="b34aa-108">Cmdlets de regra de fluxo de correio adicionais: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (acções disponíveis lista), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (condições disponíveis da lista e excepções), [TransportRuleCollection de exportação](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (regras de exportação) e [ Importar TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (regras de importação).</span><span class="sxs-lookup"><span data-stu-id="b34aa-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span> 
  

