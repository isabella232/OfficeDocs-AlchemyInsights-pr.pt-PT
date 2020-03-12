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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600391"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Aposentadoria de Legacy eDiscovery Tools

Como resultado da nova e melhorada funcionalidade eDiscovery no Microsoft 365 Compliance center, as seguintes ferramentas e comandos eDiscovery legados serão retirados nos próximos meses:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [In-Place holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração exchange.

- O Exchange Online PowerShell cmdlets que suportam In-Place eDiscovery e In-Place Holds. (Estes cmdlets são identificados coletivamente como *-MailboxSearch cmdlets.) Isto inclui os seguintes cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- A [caixa de pesquisa-mail](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet em Exchange Online PowerShell.
- As seguintes operações na API de Exchange Web Services:
    - [Caixas de Correio GetSearchableable](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Cronologia da reforma:**
- 1 de abril de 2020: Não poderá criar novas pesquisas e deter, mas ainda pode executar, editar e eliminar as pesquisas existentes por sua conta e risco. O Microsoft Support deixará de suportar o In-Place eDiscovery & Holds no EAC.

- 1 de julho de 2020: A funcionalidade In-Place eDiscovery & Holds no EAC será colocada num modo de leitura. Isto significa que só poderá remover as pesquisas e reposições existentes.

**Para mais informações, consulte:**

 - [Migrar legado eDiscovery procura e mantém-se no centro de conformidade da Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Reforma das ferramentas eDiscovery legados](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQs sobre in-place eDiscovery e In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



