---
title: Sender não recebe e-mail enviado para o grupo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872058"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="9b00f-102">Sender não recebe e-mail enviado para o grupo Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9b00f-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="9b00f-103">Por predefinição, o remetente de uma mensagem de correio eletrónico para um grupo Microsoft 365 não recebe uma cópia da mensagem na sua Caixa de Entrada, mesmo que o remetente seja membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="9b00f-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="9b00f-104">Utilize este comando EXO PowerShell para permitir que o remetente receba uma cópia de cada e-mail que enviam para o grupo Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="9b00f-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="9b00f-105">Para ativar a definição de todas as caixas de correio de uma só vez:</span><span class="sxs-lookup"><span data-stu-id="9b00f-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="9b00f-106">**Nota** As alterações a esta configuração demoram até uma hora a produzir efeitos.</span><span class="sxs-lookup"><span data-stu-id="9b00f-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>