---
title: Activar a auditoria de caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736264"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="4864e-102">Activar a auditoria de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="4864e-102">Enable mailbox auditing</span></span>

<span data-ttu-id="4864e-103">Para activar a auditoria de caixa de correio para um único utilizador ou toda uma organização tem de ser executados de Shell Remota do energia os cmdlets seguintes:</span><span class="sxs-lookup"><span data-stu-id="4864e-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="4864e-104">**Utilizador único**</span><span class="sxs-lookup"><span data-stu-id="4864e-104">**Single User**</span></span>
  
<span data-ttu-id="4864e-105">Set-Mailbox - identidade "Joana Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="4864e-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="4864e-106">**Organização**</span><span class="sxs-lookup"><span data-stu-id="4864e-106">**Organization**</span></span>
  
<span data-ttu-id="4864e-107">Get-Mailbox - ResultSize ilimitado - filtrar {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="4864e-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="4864e-108">Obter mais informações</span><span class="sxs-lookup"><span data-stu-id="4864e-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

