---
title: 2419-incapaz de permitir a auditoria
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767610"
---
# <a name="unable-to-enable-unified-auditing"></a>Incapaz de permitir auditorias unificadas

Quando tentar ativar uma auditoria unificada para a sua organização, poderá receber um erro semelhante ao seguinte:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Para resolver esta questão, siga estes passos:

1. [Ligue-se a Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Executar o seguinte cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Aguarde 60 minutos para que a definição anterior entre em vigor.

4. Executar o seguinte comando em Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Para obter informações adicionais, consulte os seguintes artigos:

- [Conecte-se a Exchange Online PowerShell usando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ligue a pesquisa de registo de auditoria ou desligada](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
