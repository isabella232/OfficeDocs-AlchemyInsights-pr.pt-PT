---
title: 2419-não é possível-para-activar-auditoria
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065685"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="89622-102">Não é possível activar a auditoria unificado</span><span class="sxs-lookup"><span data-stu-id="89622-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="89622-103">Quando tenta activar a auditoria unificado para a sua organização do Office 365, poderá receber um erro semelhante à seguinte:</span><span class="sxs-lookup"><span data-stu-id="89622-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="89622-104">Para resolver este problema, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="89622-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="89622-105">[Liga ao Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="89622-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="89622-106">Execute o cmdlet seguinte:</span><span class="sxs-lookup"><span data-stu-id="89622-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="89622-107">Espere durante 60 minutos para a anterior definição tenha efeito.</span><span class="sxs-lookup"><span data-stu-id="89622-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="89622-108">Execute o seguinte comando no PowerShell Online do Exchange:</span><span class="sxs-lookup"><span data-stu-id="89622-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="89622-109">Para obter informações adicionais, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="89622-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="89622-110">Ligar ao Exchange PowerShell Online, utilizando a autenticação multi-factores</span><span class="sxs-lookup"><span data-stu-id="89622-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="89622-111">Activar ou desactivar a procura de registo de auditoria do Office 365</span><span class="sxs-lookup"><span data-stu-id="89622-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
