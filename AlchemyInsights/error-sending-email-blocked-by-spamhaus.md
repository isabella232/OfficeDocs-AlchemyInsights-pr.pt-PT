---
title: Erro de envio de e-mail bloqueado por SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783814"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="13920-102">Erro de envio de e-mail: Anfitrião do cliente bloqueado usando Spamhaus</span><span class="sxs-lookup"><span data-stu-id="13920-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="13920-103">O endereço IP que enviou a mensagem está numa lista de blocos propriedade [do Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="13920-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="13920-104">As razões para ser bloqueado pelo Spamhaus incluem contas comprometidas, máquinas comprometidas que partilham um endereço IP público e políticas de Fornecedor de Serviços de Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="13920-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="13920-105">Possíveis correções são:</span><span class="sxs-lookup"><span data-stu-id="13920-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="13920-106">Para mensagens de entrada bloqueadas onde controla o servidor de e-mail de origem, tem de determinar a causa e remover o bloco do website do Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="13920-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="13920-107">Para mensagens de entrada bloqueadas onde o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site do Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="13920-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="13920-108">Se o endereço IP estiver na Lista de Bloqueio de Política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remover o endereço do PBL.</span><span class="sxs-lookup"><span data-stu-id="13920-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="13920-109">Para mensagens de saída bloqueadas do seu domínio ligado à Microsoft, pode receber este erro se as mensagens forem encaminhadas através de um serviço de terceira parte.</span><span class="sxs-lookup"><span data-stu-id="13920-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="13920-110">Pode utilizar uma ferramenta de procuração whois para encontrar o proprietário do endereço IP bloqueado.</span><span class="sxs-lookup"><span data-stu-id="13920-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
