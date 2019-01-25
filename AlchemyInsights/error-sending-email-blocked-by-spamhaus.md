---
title: Erro ao enviar correio electrónico bloqueado pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483861"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="e6f1c-102">Erro ao enviar uma mensagem de correio electrónico: bloqueado utilizando Spamhaus de anfitrião de cliente</span><span class="sxs-lookup"><span data-stu-id="e6f1c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="e6f1c-p101">O endereço IP que enviou a mensagem está numa lista de bloqueio pertencente a [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razões para a ser bloqueado pela Spamhaus incluem contas comprometidas, comprometida computadores a partilhar um endereço IP público e políticas do fornecedor de serviços Internet (ISP). Correcções possíveis são:</span><span class="sxs-lookup"><span data-stu-id="e6f1c-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="e6f1c-106">Para mensagens de entrada bloqueadas para onde pode controlar o servidor de correio electrónico de origem do Office 365, tem de determinar a causa e remover o bloqueio de Web site da Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="e6f1c-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="e6f1c-p102">Para mensagens de entrada bloqueadas para Office 365, se o endereço IP de origem pertence a outra pessoa, o proprietário do endereço tem de remover o bloqueio de Web site da Spamhaus. Se o endereço IP na lista de bloco de política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remova o endereço de PBL.</span><span class="sxs-lookup"><span data-stu-id="e6f1c-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="e6f1c-p103">Para mensagens de saída bloqueadas do domínio do Office 365, poderá receber este erro se as mensagens são encaminhadas através de um serviço da parte 3. Pode utilizar uma ferramenta de pesquisa WHOIS para encontrar o proprietário de endereços IP bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e6f1c-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

