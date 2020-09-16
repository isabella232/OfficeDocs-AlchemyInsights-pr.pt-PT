---
title: Eventos de resolução de problemas a partir de e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658745"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="16ab4-102">Eventos de resolução de problemas a partir de e-mail</span><span class="sxs-lookup"><span data-stu-id="16ab4-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="16ab4-103">Verifique se a funcionalidade está ativada para a caixa de correio: \*\*Get-EventsFromEmailConfiguration -Identidade <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="16ab4-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="16ab4-104">Em seguida, veja os registos 'Eventos do Email' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="16ab4-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="16ab4-105">Nos registos 'Eventos do Email', encontre o InternetMessageId que corresponda ao item na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="16ab4-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="16ab4-106">O TrustScore determina se o artigo é adicionado ou não.</span><span class="sxs-lookup"><span data-stu-id="16ab4-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="16ab4-107">Os eventos só serão adicionados se o TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="16ab4-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="16ab4-108">O TrustScore é determinado pelas propriedades SPF, Dkim ou Dmarc, que estão no Cabeçalho de Mensagem.</span><span class="sxs-lookup"><span data-stu-id="16ab4-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="16ab4-109">Para ver estas propriedades:</span><span class="sxs-lookup"><span data-stu-id="16ab4-109">To view these properties:</span></span>

<span data-ttu-id="16ab4-110">**Perspetivas de Ambiente de Trabalho**</span><span class="sxs-lookup"><span data-stu-id="16ab4-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="16ab4-111">Abra o item</span><span class="sxs-lookup"><span data-stu-id="16ab4-111">Open the item</span></span>
- <span data-ttu-id="16ab4-112">File -> Properties -> Cabeçalhos de Internet</span><span class="sxs-lookup"><span data-stu-id="16ab4-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="16ab4-113">ou</span><span class="sxs-lookup"><span data-stu-id="16ab4-113">or</span></span>

<span data-ttu-id="16ab4-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="16ab4-114">**MFCMapi**</span></span>

- <span data-ttu-id="16ab4-115">Navegue para o item na caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="16ab4-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="16ab4-116">Procure por PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="16ab4-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="16ab4-117">Estas propriedades são determinadas e registadas durante o transporte e encaminhamento.</span><span class="sxs-lookup"><span data-stu-id="16ab4-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="16ab4-118">Para uma resolução de problemas, poderá ter de acompanhar o Apoio ao Transporte sobre as falhas em SPF, DKIM e.ou DMARC.</span><span class="sxs-lookup"><span data-stu-id="16ab4-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>