---
title: Precisa de ajuda com os limites de envio de e-mails?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836290"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="244e5-102">Precisa de ajuda com os limites de envio de e-mails?</span><span class="sxs-lookup"><span data-stu-id="244e5-102">Need help with email sending limits?</span></span>

<span data-ttu-id="244e5-103">Abaixo encontram-se os **limites de envio predefinidos** aplicados ao serviço.</span><span class="sxs-lookup"><span data-stu-id="244e5-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="244e5-104">Pode encontrar mais informações documentadas sobre estes limites [aqui](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="244e5-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="244e5-105">Para evitar a entrega de mensagens em massa não solicitadas, aplicamos **limites de taxa de destinatários por utilizador a todas as mensagens internas e externas**.</span><span class="sxs-lookup"><span data-stu-id="244e5-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="244e5-106">Em todos os SKUs, este limite é de **10.000 destinatários por dia**.</span><span class="sxs-lookup"><span data-stu-id="244e5-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="244e5-107">Os clientes que precisem de enviar e-mails comerciais legítimos em massa (por exemplo, newsletters de clientes) devem utilizar fornecedores de terceiros especializados nestes serviços.</span><span class="sxs-lookup"><span data-stu-id="244e5-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="244e5-108">**Nota**: Assim que o limite da taxa de destinatários seja atingido, as mensagens não podem ser enviadas da caixa de correio até ao número de destinatários que receberam mensagens nas últimas 24 horas descer abaixo do limite.</span><span class="sxs-lookup"><span data-stu-id="244e5-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="244e5-109">O utilizador não conseguirá enviar mensagens até essa altura.</span><span class="sxs-lookup"><span data-stu-id="244e5-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="244e5-110">O limite da taxa de mensagens de **30 mensagens por minuto** é aplicado em todos os SKUs.</span><span class="sxs-lookup"><span data-stu-id="244e5-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="244e5-111">Isto determina o número de mensagens que um utilizador pode enviar a partir da sua conta do Exchange Online num período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="244e5-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="244e5-112">O **número máximo de destinatários permitidos nos campos Para, Cc e Bcc** para uma única mensagem de e-mail, em todos os SKUs, é de **1000 destinatários**.</span><span class="sxs-lookup"><span data-stu-id="244e5-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="244e5-113">Para personalizar este limite, aceda [aqui](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="244e5-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
