---
title: Não pode enviar/receber e-mail para/do Office 365 por causa do desactivamento TLS 1.0 e TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747120"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="7f8e5-102">Não pode enviar/receber e-mail para/do Office 365 por causa do desactivamento TLS 1.0 e TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="7f8e5-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="7f8e5-103">Como confirmado pelo post do centro de mensagens MC229914, TLS 1.0 e TLS 1.1 deprecação começaram a aplicar para exchange online fluxo de fluxo de fluxo de correio.</span><span class="sxs-lookup"><span data-stu-id="7f8e5-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="7f8e5-104">Em breve, o Office 365 deixará de aceitar ligações de e-mail TLS 1.0 e TLS 1.1 de fontes externas.</span><span class="sxs-lookup"><span data-stu-id="7f8e5-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="7f8e5-105">Além disso, o Exchange Online nunca usará TLS 1.0 ou 1.1 para enviar e-mail de saída.</span><span class="sxs-lookup"><span data-stu-id="7f8e5-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="7f8e5-106">Se estiver a enfrentar problemas por causa de desativação de TLS 1.0 ou 1.1, poderá sofrer um dos seguintes erros.</span><span class="sxs-lookup"><span data-stu-id="7f8e5-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="7f8e5-107">O remetente está a recuperar o NDR - '421 4.4.2 A ligação caiu devido ao SocketError'</span><span class="sxs-lookup"><span data-stu-id="7f8e5-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="7f8e5-108">Erro no servidor de visualização de filas de instalações que está a enviar e-mail para o Agente 365- '421 4.4.2 A ligação caiu devido ao SocketError'</span><span class="sxs-lookup"><span data-stu-id="7f8e5-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="7f8e5-109">Erro no Registo do [Protocolo](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) de Ligação no servidor enviando e-mail para o Office 365-TLS negociação falhou com erro SocketError</span><span class="sxs-lookup"><span data-stu-id="7f8e5-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="7f8e5-110">Erro no registo do protocolo de envio ou receção - '451 5.7.3 Deve emitir primeiro um comando STARTTLS'</span><span class="sxs-lookup"><span data-stu-id="7f8e5-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="7f8e5-111">Se experimentar algum dos erros acima, certifique-se de que o servidor que está a enviar ou a receber e-mail tem OLS 1.2 ativado, verificando as seguintes chaves de registo...</span><span class="sxs-lookup"><span data-stu-id="7f8e5-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="7f8e5-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Cliente] **"DisabledByDefault"=dword:0000000 "Enabled"=dword:0000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="7f8e5-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="7f8e5-113">Se efetuar qualquer alteração nas teclas de registo acima para ativar o TLS 1.2, reinicie o servidor para que as alterações produzam efeitos.</span><span class="sxs-lookup"><span data-stu-id="7f8e5-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="7f8e5-114">Certifique-se também de que tem as últimas atualizações do Windows e Exchange instaladas.</span><span class="sxs-lookup"><span data-stu-id="7f8e5-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="7f8e5-115">Para mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="7f8e5-115">For more information, see:</span></span>

- [<span data-ttu-id="7f8e5-116">Orientação TLS do Servidor de Intercâmbio, parte 1: Preparação para TLS 1.2 - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="7f8e5-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="7f8e5-117">Linha de orientação do Servidor de Intercâmbio Parte 2: Ativar TLS 1.2 e identificar clientes que não o utilizam - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="7f8e5-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="7f8e5-118">Compreender cenários de e-mail se as versões TLS não puderem ser acordadas com o Exchange Online - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="7f8e5-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
