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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Não pode enviar/receber e-mail para/do Office 365 por causa do desactivamento TLS 1.0 e TLS 1.1

Como confirmado pelo post do centro de mensagens MC229914, TLS 1.0 e TLS 1.1 deprecação começaram a aplicar para exchange online fluxo de fluxo de fluxo de correio. Em breve, o Office 365 deixará de aceitar ligações de e-mail TLS 1.0 e TLS 1.1 de fontes externas. Além disso, o Exchange Online nunca usará TLS 1.0 ou 1.1 para enviar e-mail de saída. Se estiver a enfrentar problemas por causa de desativação de TLS 1.0 ou 1.1, poderá sofrer um dos seguintes erros.

- O remetente está a recuperar o NDR - '421 4.4.2 A ligação caiu devido ao SocketError'
- Erro no servidor de visualização de filas de instalações que está a enviar e-mail para o Agente 365- '421 4.4.2 A ligação caiu devido ao SocketError'
- Erro no Registo do [Protocolo](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) de Ligação no servidor enviando e-mail para o Office 365-TLS negociação falhou com erro SocketError
- Erro no registo do protocolo de envio ou receção - '451 5.7.3 Deve emitir primeiro um comando STARTTLS'

Se experimentar algum dos erros acima, certifique-se de que o servidor que está a enviar ou a receber e-mail tem OLS 1.2 ativado, verificando as seguintes chaves de registo...

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Cliente] **"DisabledByDefault"=dword:0000000 "Enabled"=dword:0000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Se efetuar qualquer alteração nas teclas de registo acima para ativar o TLS 1.2, reinicie o servidor para que as alterações produzam efeitos. Certifique-se também de que tem as últimas atualizações do Windows e Exchange instaladas.

Para mais informações, consulte:

- [Orientação TLS do Servidor de Intercâmbio, parte 1: Preparação para TLS 1.2 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Linha de orientação do Servidor de Intercâmbio Parte 2: Ativar TLS 1.2 e identificar clientes que não o utilizam - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Compreender cenários de e-mail se as versões TLS não puderem ser acordadas com o Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
