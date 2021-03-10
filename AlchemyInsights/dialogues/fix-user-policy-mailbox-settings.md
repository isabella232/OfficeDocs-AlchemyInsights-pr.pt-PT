---
title: Corrigir as definições da política do utilizador/caixa de correio
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695905"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="ff7c9-102">Corrigir as definições da política do utilizador/caixa de correio</span><span class="sxs-lookup"><span data-stu-id="ff7c9-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="ff7c9-103">As definições de correio publicitário não solicitado na caixa de correio afetaram esta mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff7c9-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="ff7c9-104">Para rever as definições, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ff7c9-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="ff7c9-105">Launch Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="ff7c9-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="ff7c9-106">Para mais informações, consulte [Abrir a Shell de Gestão de Câmbios.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="ff7c9-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="ff7c9-107">Executar este comando (utilizando o endereço de e-mail do utilizador):  **obter caixa de correio eletrónicoconfiguration -identidade "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="ff7c9-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="ff7c9-108">Verifique se o endereço de e-mail do remetente faz parte de **TrustedSendersAndDomains** ou **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="ff7c9-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="ff7c9-109">Se o endereço de e-mail estiver numa das listas, poderá ter de o remover.</span><span class="sxs-lookup"><span data-stu-id="ff7c9-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="ff7c9-110">Para saber mais, consulte [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="ff7c9-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
