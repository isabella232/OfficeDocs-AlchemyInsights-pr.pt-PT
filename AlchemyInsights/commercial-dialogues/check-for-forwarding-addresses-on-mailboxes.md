---
title: Verifique se há endereços de encaminhamento nas caixas de correio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403322"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="d27ce-102">Verifique se há endereços de encaminhamento nas caixas de correio</span><span class="sxs-lookup"><span data-stu-id="d27ce-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="d27ce-103">Por vezes, os hackers encaminham as mensagens de e-mail dos utilizadores para si mesmos, por isso, primeiro, vamos verificar se enviamos endereços e regras na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d27ce-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="d27ce-104">Depois vamos verificar os registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d27ce-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="d27ce-105">Aqui está como verificar se os endereços de encaminhamento:</span><span class="sxs-lookup"><span data-stu-id="d27ce-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="d27ce-106">Selecione **utilizadores**  >  **Utilizadores Ative**.</span><span class="sxs-lookup"><span data-stu-id="d27ce-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="d27ce-107">Selecione o utilizador cuja conta foi comprometida.</span><span class="sxs-lookup"><span data-stu-id="d27ce-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="d27ce-108">No flyout que aparece, expanda **as Definições de Correio** e, em seguida, clique em **Editar** para **reencaminhamento de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="d27ce-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="d27ce-109">Remova quaisquer endereços de reencaminhamento que não reconheça.</span><span class="sxs-lookup"><span data-stu-id="d27ce-109">Remove any forwarding addresses you don't recognize.</span></span>