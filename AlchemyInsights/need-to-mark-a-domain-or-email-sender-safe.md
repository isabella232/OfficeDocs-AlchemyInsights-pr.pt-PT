---
title: Precisa marcar um domínio ou e-mail cofre?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281182"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="495bb-102">Precisa marcar um domínio ou e-mail cofre?</span><span class="sxs-lookup"><span data-stu-id="495bb-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="495bb-103">A utilização de listas de **remetentes seguras não é recomendada,** uma vez que abre a sua organização a ataques de spam, phish e falsificação.</span><span class="sxs-lookup"><span data-stu-id="495bb-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="495bb-104">No entanto, se houver um requisito de negócio, **recomendamos** a utilização de Regras de Fluxo de **[Correio](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para o mesmo.</span><span class="sxs-lookup"><span data-stu-id="495bb-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="495bb-105">A nossa orientação garante a autenticação do remetente (verifica que o domínio de envio não está a ser falsificado).</span><span class="sxs-lookup"><span data-stu-id="495bb-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="495bb-106">**Nota:** Não recomendamos gerir falsos positivos utilizando listas de remetentes seguras, porque exceções à filtragem de spam podem abrir a sua organização a ataques de segurança.</span><span class="sxs-lookup"><span data-stu-id="495bb-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="495bb-107">Se o seu utilizador(s) receber mensagens incorretamente marcadas como correio publicitário não solicitado ou lixo, por **[favor, informe mensagens e ficheiros para a Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="495bb-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="495bb-108">Os remetentes seguros no Outlook, a lista de remetentes permitidas ou a lista de domínios permitidas nas políticas anti-correio publicitário não solicitado **devem ser evitadas** porque os remetentes contornam todos os spam, spoof e phish protection, e a autenticação do remetente (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="495bb-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="495bb-109">Este método é melhor utilizado apenas para testes temporários.</span><span class="sxs-lookup"><span data-stu-id="495bb-109">This method is best used for temporary testing only.</span></span>
