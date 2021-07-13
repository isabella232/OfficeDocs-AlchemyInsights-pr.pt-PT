---
title: Grupo de relay de saída
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381859"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="3213b-102">Grupo de relay de saída</span><span class="sxs-lookup"><span data-stu-id="3213b-102">Outbound relay pool</span></span>

<span data-ttu-id="3213b-103">A Microsoft está a fazer algumas alterações à configuração do relaying ou encaminhamento de e-mail através Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3213b-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="3213b-104">As mensagens em determinados cenários são re encaminhadas ou relayadas através Microsoft 365 através de um grupo de relay especial.</span><span class="sxs-lookup"><span data-stu-id="3213b-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="3213b-105">As mensagens enviadas através do grupo de relay podem aparecer na pasta de e-mail de lixo do destinatário.</span><span class="sxs-lookup"><span data-stu-id="3213b-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="3213b-106">Para obter mais informações, consulte [ações de entrega de saída](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="3213b-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="3213b-107">Para evitar um cenário com o grupo de reenainhamento, certifique-se de que as mensagens reencainhadas/reencainhadas cumprem um dos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="3213b-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="3213b-108">O remetente de saída é um domínio aceite do inquilino.</span><span class="sxs-lookup"><span data-stu-id="3213b-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="3213b-109">O SPF (Sender Policy Framework) passa quando a mensagem chega Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3213b-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="3213b-110">O DKIM (DomainKeys Identified Mail) no domínio do remetente P2 passa quando a mensagem é enviada Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3213b-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="3213b-111">As mensagens que cumprem os critérios descritos acima não são reencalecidas através do grupo de reenais.</span><span class="sxs-lookup"><span data-stu-id="3213b-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="3213b-112">Se o registo MX do seu domínio estiver apontado para um servidor de terceiros ou no local, utilize a filtragem melhorada para se certificar de que a validação de SPF está correta para o e-mail de entrada e para evitar o envio de e-mail através do agrupamento de relay.</span><span class="sxs-lookup"><span data-stu-id="3213b-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="3213b-113">**Como podemos saber se estamos a ser afetados pelo grupo de relay?**</span><span class="sxs-lookup"><span data-stu-id="3213b-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="3213b-114">Se os seus e-mails re encaminhados ou re encaminhados utilizarem um dos critérios acima, as mensagens não serão relayadas através do grupo de relay.</span><span class="sxs-lookup"><span data-stu-id="3213b-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="3213b-115">No entanto, se uma mensagem for enviada através de um conjunto de relay, o IP do servidor de saída está no intervalo 40.95.0.0/16 e o nome do servidor de saída inclui **rly** no nome.</span><span class="sxs-lookup"><span data-stu-id="3213b-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

