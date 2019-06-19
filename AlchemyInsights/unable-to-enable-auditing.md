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
# <a name="unable-to-enable-unified-auditing"></a>Não é possível activar a auditoria unificado

Quando tenta activar a auditoria unificado para a sua organização do Office 365, poderá receber um erro semelhante à seguinte:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Para resolver este problema, siga estes passos:

1. [Liga ao Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Execute o cmdlet seguinte:

   ```
   Enable-OrganizationCustomization
   ```

3. Espere durante 60 minutos para a anterior definição tenha efeito.

4. Execute o seguinte comando no PowerShell Online do Exchange:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Para obter informações adicionais, consulte os seguintes artigos:

- [Ligar ao Exchange PowerShell Online, utilizando a autenticação multi-factores](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activar ou desactivar a procura de registo de auditoria do Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
