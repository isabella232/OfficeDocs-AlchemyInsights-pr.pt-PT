---
title: Precisa de ajuda com os limites de envio de e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357870"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="6a1e9-102">Precisa de ajuda com os limites de envio de e-mail?</span><span class="sxs-lookup"><span data-stu-id="6a1e9-102">Need help with email sending limits?</span></span>

<span data-ttu-id="6a1e9-103">Abaixo estão os **limites de envio de by-design** imposto no serviço.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="6a1e9-104">Mais informações sobre estes limites estão [aqui](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)documentadas.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="6a1e9-105">Para desencorajar a entrega de mensagens a granel não solicitadas, aplicamos limites de taxa de destinatário por utilizador **a todas as mensagens de saída e internas**.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="6a1e9-106">Em todas as SKUs, este limite é **de 10.000 destinatários por dia.**</span><span class="sxs-lookup"><span data-stu-id="6a1e9-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="6a1e9-107">Os clientes que necessitem de enviar e-mails comerciais legítimos a granel (por exemplo, newsletters de clientes) devem utilizar fornecedores de terceiros especializados nestes serviços.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="6a1e9-108">**Nota**: Uma vez atingido o limite de taxa de destinatário, as mensagens não podem ser enviadas da caixa de correio até que o número de destinatários que foram enviados nas últimas 24 horas cai abaixo do limite.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="6a1e9-109">O utilizador não poderá enviar mensagens até esse ponto.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="6a1e9-110">O limite da taxa de mensagem de **30 mensagens por minuto** é aplicado em todas as SKUs.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="6a1e9-111">Isto determina quantas mensagens um utilizador pode enviar da sua conta Exchange Online num período determinado.</span><span class="sxs-lookup"><span data-stu-id="6a1e9-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="6a1e9-112">O **número máximo de destinatários permitidos nos** campos To, Cc e Bcc para uma única mensagem de e-mail, em todas as SKUs, é de **1000 destinatários.**</span><span class="sxs-lookup"><span data-stu-id="6a1e9-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="6a1e9-113">Para personalizar este limite, vá [aqui.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="6a1e9-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
