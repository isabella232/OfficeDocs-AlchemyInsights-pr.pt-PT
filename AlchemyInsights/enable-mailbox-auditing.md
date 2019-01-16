---
title: Activar a auditoria de caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28305197"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="0ee27-102">Activar a auditoria de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="0ee27-102">Enable mailbox auditing</span></span>

<span data-ttu-id="0ee27-103">Para activar a auditoria de caixa de correio para um único utilizador ou toda uma organização tem de ser executados de Shell Remota do energia os cmdlets seguintes:</span><span class="sxs-lookup"><span data-stu-id="0ee27-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="0ee27-104">**Utilizador único**</span><span class="sxs-lookup"><span data-stu-id="0ee27-104">**Single User**</span></span>
  
<span data-ttu-id="0ee27-105">Set-Mailbox - identidade "Joana Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0ee27-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="0ee27-106">**Organization**</span><span class="sxs-lookup"><span data-stu-id="0ee27-106">**Organization**</span></span>
  
<span data-ttu-id="0ee27-107">Get-Mailbox - ResultSize ilimitado - filtrar {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0ee27-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="0ee27-108">Obter mais informações</span><span class="sxs-lookup"><span data-stu-id="0ee27-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

