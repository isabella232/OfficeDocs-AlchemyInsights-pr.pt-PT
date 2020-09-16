---
title: Email de saída para pasta Junk Email
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769194"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="405db-102">Email de saída para pasta Junk Email</span><span class="sxs-lookup"><span data-stu-id="405db-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="405db-103">Se estiver a ver mensagens de saída a serem marcadas como Lixo, faça os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="405db-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="405db-104">Se ainda não o fez, considere [configurar notificações de políticas de spam de saída.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="405db-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="405db-105">Utilize [o rastreio da mensagem](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) para ver se a mensagem de saída tem o valor do evento **Spam** com o detalhe adicional: **Utilize um pool de entrega de alto risco**.</span><span class="sxs-lookup"><span data-stu-id="405db-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="405db-106">Para estas mensagens, consulte o conteúdo da mensagem para ver o que pode ser considerado spam.</span><span class="sxs-lookup"><span data-stu-id="405db-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="405db-107">Por exemplo, as assinaturas podem, por vezes, causar problemas a muitos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="405db-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="405db-108">Se tiver vários exemplos de mensagens legítimas de saída que estão a ser marcadas como Junk, abra um bilhete de apoio e peça ao agente de suporte para submeter as suas mensagens como falsos positivos aos nossos analistas de spam.</span><span class="sxs-lookup"><span data-stu-id="405db-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="405db-109">Esteja preparado para fornecer mensagens de amostra que incluam todos os cabeçalhos de mensagens.</span><span class="sxs-lookup"><span data-stu-id="405db-109">Be prepared to provide sample messages that include all message headers.</span></span>
