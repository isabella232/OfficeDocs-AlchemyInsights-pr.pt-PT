---
title: Aposentadoria de Legacy eDiscovery Tools
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902631"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Aposentadoria de Legacy eDiscovery Tools

Como resultado da nova e melhorada funcionalidade eDiscovery no Microsoft 365 Compliance center, as seguintes ferramentas e comandos eDiscovery legados serão retirados nos próximos meses:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no Centro de Administração Exchange.

- Os cmdlets Exchange Online PowerShell que suportam in-place eDiscovery e In-Place Holds. (Estes cmdlets são identificados colectivamente como cmdlets *-MailboxSearch.) Isto inclui os seguintes cmdlets:

    - [Novo MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- O [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) em Exchange Online PowerShell.
- As seguintes operações na API de Serviços Web de Câmbio:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [EDiscovery avançado v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Cronologia da reforma:**
- **1 de julho de 2020** Já não é possível criar novas pesquisas e detém, mas pode executar, editar e eliminar as pesquisas existentes por sua conta e risco. O Microsoft Support já não suporta in-place eDiscovery & Holds no EAC.
    
- **1 de outubro de 2020** In-Place eDiscovery & A funcionalidade Holds no EAC será colocada no modo apenas de leitura, pelo que só pode remover as pesquisas e os suportes existentes.

**Para mais informações, consulte:**

 - [Migrar pesquisas eDiscovery legacy e detém para o centro de conformidade Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Aposentadoria de ferramentas eDiscovery legacy](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Perguntas frequentes sobre in-place eDiscovery e In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



