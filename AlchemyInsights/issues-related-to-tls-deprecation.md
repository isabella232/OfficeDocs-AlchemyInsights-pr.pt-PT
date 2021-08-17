---
title: Não é possível enviar/receber e-mail de/para Office 365 devido à desativação do TLS 1.0 e TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054917"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Não é possível enviar/receber e-mail de/para Office 365 devido à desativação do TLS 1.0 e TLS 1.1

Conforme confirmado pelo centro de mensagens mc229914, a preterição TLS 1.0 e TLS 1.1 começou a impor os pontos finais do Exchange Online fluxo de correio. Em Office 365 deixarão de aceitar ligações de e-mail TLS 1.0 e TLS 1.1 a partir de origens externas. Além disso, Exchange Online utilizará TLS 1.0 ou 1.1 para enviar e-mails de saída. Se estiver a ter problemas devido à desativação TLS 1.0 ou 1.1, poderá deparar-se com um dos seguintes erros:

- O remetente está a ser ressalto pelo NDR - '421 4.4.2 A ligação deixou de ser lida devido a SocketError'
- Erro no Visualização de Fila do Servidor no Local que está a enviar e-mails para o Agente 365- '421 4.4.2 Ligação abandonada devido a SocketError'
- Erro no registo [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) Enviar Protocolo de Conector no servidor que envia e-mail para o Office 365- A negociação de TLS falhou com o erro SocketError
- Erro no registo enviar ou receber protocolo de conexão - '451 5.7.3 Tem de emitir primeiro um comando STARTTLS'

Se detetou algum dos erros acima, certifique-se de que o servidor que está a enviar ou receber e-mails tem o TLS 1.2 ativado ao verificar as seguintes chaves de registo:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Se efetuar alterações às chaves de registo acima para ativar o TLS 1.2, reinicie o servidor para que as alterações entrem em vigor. Certifique-se também de que tem as atualizações Windows e Exchange atualizações mais recentes instaladas.

Para mais informações, consulte:

- [Exchange Server Orientação TLS, parte 1: Preparar-se para o TLS 1.2 – Comunidade Tecnológica Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Orientação TLS Parte 2: Ativar o TLS 1.2 e Identificar Clientes que Não o Utilizam - Comunidade Tecnológica Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Compreender cenários de e-mail se não for possível concordar com as versões TLS Exchange Online - Comunidade Tecnológica Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
