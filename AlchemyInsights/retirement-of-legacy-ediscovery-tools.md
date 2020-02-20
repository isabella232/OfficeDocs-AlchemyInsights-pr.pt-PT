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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157676"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="b7f8c-102">Aposentadoria de Legacy eDiscovery Tools</span><span class="sxs-lookup"><span data-stu-id="b7f8c-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="b7f8c-103">Como resultado da nova e melhorada funcionalidade eDiscovery no Microsoft 365 Compliance center, as seguintes ferramentas e comandos eDiscovery legados serão retirados nos próximos meses:</span><span class="sxs-lookup"><span data-stu-id="b7f8c-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="b7f8c-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) e [In-Place holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) no centro de administração exchange.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="b7f8c-105">O Exchange Online PowerShell cmdlets que suportam In-Place eDiscovery e In-Place Holds.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="b7f8c-106">(Estes cmdlets são identificados coletivamente como \*-MailboxSearch cmdlets.) Isto inclui os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="b7f8c-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="b7f8c-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="b7f8c-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="b7f8c-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="b7f8c-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="b7f8c-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="b7f8c-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="b7f8c-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="b7f8c-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="b7f8c-111">A [caixa de pesquisa-mail](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet em Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="b7f8c-112">As seguintes operações na API de Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="b7f8c-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="b7f8c-113">Caixas de Correio GetSearchableable</span><span class="sxs-lookup"><span data-stu-id="b7f8c-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="b7f8c-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b7f8c-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="b7f8c-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b7f8c-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="b7f8c-116">Office 365 Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="b7f8c-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="b7f8c-117">**Cronologia da reforma:**</span><span class="sxs-lookup"><span data-stu-id="b7f8c-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="b7f8c-118">1 de abril de 2020: Não poderá criar novas pesquisas e deter, mas ainda pode executar, editar e eliminar as pesquisas existentes por sua conta e risco.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="b7f8c-119">O Microsoft Support deixará de suportar o In-Place eDiscovery & Holds no EAC.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="b7f8c-120">1 de julho de 2020: A funcionalidade In-Place eDiscovery & Holds no EAC será colocada num modo de leitura.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="b7f8c-121">Isto significa que só poderá remover as pesquisas e reposições existentes.</span><span class="sxs-lookup"><span data-stu-id="b7f8c-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="b7f8c-122">**Para mais informações, consulte:**</span><span class="sxs-lookup"><span data-stu-id="b7f8c-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="b7f8c-123">Migrar legado eDiscovery procura e mantém-se no centro de conformidade da Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b7f8c-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="b7f8c-124">Reforma das ferramentas eDiscovery legados</span><span class="sxs-lookup"><span data-stu-id="b7f8c-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="b7f8c-125">FAQs sobre in-place eDiscovery e In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="b7f8c-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



