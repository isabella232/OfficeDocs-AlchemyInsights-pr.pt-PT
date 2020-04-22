---
title: Ativar a auditoria da caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703582"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="909b1-102">Ativar a auditoria da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="909b1-102">Enable mailbox auditing</span></span>

<span data-ttu-id="909b1-103">Para ativar a auditoria da Caixa de Correio seletiva mente para um único utilizador ou para uma organização inteira, os seguintes cmdlets devem ser executados a partir da Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="909b1-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="909b1-104">**Utilizador Único**</span><span class="sxs-lookup"><span data-stu-id="909b1-104">**Single User**</span></span>
  
<span data-ttu-id="909b1-105">Set-Mailbox -Identidade "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="909b1-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="909b1-106">**Organização**</span><span class="sxs-lookup"><span data-stu-id="909b1-106">**Organization**</span></span>
  
<span data-ttu-id="909b1-107">Caixa de correio -ResultSize Ilimitado -Filter {RecipientTypeDetails -eq "UserMailbox"} Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="909b1-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="909b1-108">Saiba mais</span><span class="sxs-lookup"><span data-stu-id="909b1-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

