---
title: Aposentadoria de Legacy eDiscovery Tools
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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798560"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="6803d-102">Aposentadoria de Legacy eDiscovery Tools</span><span class="sxs-lookup"><span data-stu-id="6803d-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="6803d-103">Como resultado da nova e melhorada funcionalidade eDiscovery no Microsoft 365 Compliance center, as seguintes ferramentas e comandos eDiscovery legados serão retirados nos próximos meses:</span><span class="sxs-lookup"><span data-stu-id="6803d-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="6803d-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no Centro de Administração Exchange.</span><span class="sxs-lookup"><span data-stu-id="6803d-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="6803d-105">Os cmdlets Exchange Online PowerShell que suportam In-Place eDiscovery e In-Place Holds.</span><span class="sxs-lookup"><span data-stu-id="6803d-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="6803d-106">(Estes cmdlets são identificados colectivamente como cmdlets \*-MailboxSearch.) Isto inclui os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="6803d-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="6803d-107">Novo MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6803d-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="6803d-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6803d-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="6803d-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6803d-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="6803d-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6803d-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="6803d-111">O [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) em Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6803d-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="6803d-112">As seguintes operações na API de Serviços Web de Câmbio:</span><span class="sxs-lookup"><span data-stu-id="6803d-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="6803d-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="6803d-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="6803d-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="6803d-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="6803d-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="6803d-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="6803d-116">EDiscovery avançado v1.0</span><span class="sxs-lookup"><span data-stu-id="6803d-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="6803d-117">**Cronologia da reforma:**</span><span class="sxs-lookup"><span data-stu-id="6803d-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="6803d-118">**1 de julho de 2020** Já não é possível criar novas pesquisas e detém, mas pode executar, editar e eliminar as pesquisas existentes por sua conta e risco.</span><span class="sxs-lookup"><span data-stu-id="6803d-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="6803d-119">O Microsoft Support já não suporta In-Place & eDiscovery no EAC.</span><span class="sxs-lookup"><span data-stu-id="6803d-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="6803d-120">**1 de outubro de 2020** In-Place funcionalidade eDiscovery & Holds no EAC será colocada no modo apenas de leitura, pelo que só pode remover as pesquisas e os suportes existentes.</span><span class="sxs-lookup"><span data-stu-id="6803d-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="6803d-121">**Para mais informações, consulte:**</span><span class="sxs-lookup"><span data-stu-id="6803d-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="6803d-122">Migrar pesquisas eDiscovery legacy e detém para o centro de conformidade Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6803d-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="6803d-123">Aposentadoria de ferramentas eDiscovery legacy</span><span class="sxs-lookup"><span data-stu-id="6803d-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="6803d-124">Perguntas frequentes sobre In-Place eDiscovery e In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="6803d-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



