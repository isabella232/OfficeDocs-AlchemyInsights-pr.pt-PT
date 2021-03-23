---
title: Proteção contra ataque de backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037175"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="acc6f-102">Proteção contra ataque de backscatter</span><span class="sxs-lookup"><span data-stu-id="acc6f-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="acc6f-103">Backscatter é relatórios de não-entrega (também conhecidos como NDRs ou mensagens de ressalto) que recebe para mensagens que não enviou.</span><span class="sxs-lookup"><span data-stu-id="acc6f-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="acc6f-104">Os spammers falsificam (spoof) o **From:** endereço das suas mensagens, e muitas vezes usam endereços de e-mail reais para emprestar credibilidade às suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="acc6f-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="acc6f-105">Assim, quando os spammers enviam inevitavelmente mensagens a destinatários inexistentes, o servidor de e-mail de destino é essencialmente enganado para devolver a mensagem não entregue num NDR ao remetente forjado no endereço **From.**</span><span class="sxs-lookup"><span data-stu-id="acc6f-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="acc6f-106">Informações adicionais podem ser encontradas em [Backscatter em EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="acc6f-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="acc6f-107">**Habilitar a proteção de backscatter**</span><span class="sxs-lookup"><span data-stu-id="acc6f-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="acc6f-108">Para ativar a proteção do backscatter, siga o caminho abaixo.</span><span class="sxs-lookup"><span data-stu-id="acc6f-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="acc6f-109">**Política de > de gestão de ameaças protection.office.com > > Antispam > Selecione a política de filtro de spam e edite a política > propriedades de spam > Mark como spam > > de backscatter NDR defini-lo para "On"**</span><span class="sxs-lookup"><span data-stu-id="acc6f-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="acc6f-110">Se acredita que uma conta foi comprometida, consulte o seguinte:</span><span class="sxs-lookup"><span data-stu-id="acc6f-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="acc6f-111">Respondendo a uma conta de e-mail comprometida</span><span class="sxs-lookup"><span data-stu-id="acc6f-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="acc6f-112">Remoção de utilizadores bloqueados do portal Utilizadores Restritos no Office 365</span><span class="sxs-lookup"><span data-stu-id="acc6f-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



