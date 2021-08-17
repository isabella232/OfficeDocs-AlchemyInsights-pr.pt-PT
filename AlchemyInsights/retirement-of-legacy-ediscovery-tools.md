---
title: Desativação das Ferramentas de Deteção de Emails Legadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074685"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Desativação das Ferramentas de Deteção de Emails Legadas

Como resultado das novas e melhoradas funcionalidades da Deteção de Dados Técnicos no Microsoft 365 Centro de Conformidade, as seguintes ferramentas e comandos de Deteção de Dados Técnicos legados serão desativados nos próximos meses:

- [A Deteção de Dados Online e](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [As](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Retenção no Local no Exchange de administração.

- Os cmdlets Exchange Online PowerShell que suportam a Deteção de In-Place Deteção de In-Place Deteção de In-Place Em espera. (Estes cmdlets são identificados coletivamente como *-MailboxSearch cmdlets.) Isto inclui os seguintes cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- O [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) no Exchange Online PowerShell.
- As seguintes operações na API Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Linha de tempo para a despossão:**
- **1 de Julho de 2020** Já não pode criar novas pesquisas e reterções, mas pode executar, editar e eliminar pesquisas existentes por sua conta e risco. O Suporte da Microsoft já não suporta In-Place deTeção de Dados & no EAC.
    
- A deteção de dados In-Place de outubro de **2020** do & As funcionalidades de Deteção de Dados Automáticos no EAC serão colocadas no modo só de leitura, pelo que só poderá remover pesquisas e esperas existentes.

**Para obter mais informações, consulte:**

 - [Migrar pesquisas de Deteção de E-Centro de Conformidade do Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Desativação de ferramentas de Deteção de E-dio legadas](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FAQs sobre a deteção In-Place e a Deteção de In-Place Deteção de In-Place Deteção de E-In-Place Deteção de In-Place Deteção de In-Place Deteção](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



