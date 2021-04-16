---
title: Erro de envio de e-mail bloqueado por SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813735"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro de envio de e-mail: Anfitrião do cliente bloqueado usando Spamhaus

O endereço IP que enviou a mensagem está numa lista de blocos propriedade [do Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). As razões para ser bloqueado pelo Spamhaus incluem contas comprometidas, máquinas comprometidas que partilham um endereço IP público e políticas de Fornecedor de Serviços de Internet (ISP). Possíveis correções são:
  
- Para mensagens de entrada bloqueadas onde controla o servidor de e-mail de origem, tem de determinar a causa e remover o bloco do website do Spamhaus.

- Para mensagens de entrada bloqueadas onde o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site do Spamhaus. Se o endereço IP estiver na Lista de Bloqueio de Política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remover o endereço do PBL.

- Para mensagens de saída bloqueadas do seu domínio ligado à Microsoft, pode receber este erro se as mensagens forem encaminhadas através de um serviço de terceira parte. Pode utilizar uma ferramenta de procuração whois para encontrar o proprietário do endereço IP bloqueado.
