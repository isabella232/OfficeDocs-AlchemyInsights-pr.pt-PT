---
title: Erro ao enviar e-mail bloqueado pelo SpamHaus
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
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946775"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro ao enviar e-mail: o anfitrião cliente foi bloqueado com o Spamhaus

O endereço IP que enviou a mensagem está numa lista de bloqueios que pertence ao [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) As razões para ser bloqueado pelo Spamhaus incluem contas comprometida, máquinas comprometidos que partilham um endereço IP público e políticas do Fornecedor de Serviços Internet (ISP). As correções possíveis são:
  
- Para mensagens de receção bloqueadas onde controla o servidor de e-mail de origem, tem de determinar a causa e remover o bloqueio do site Spamhaus.

- No caso de mensagens de receção bloqueadas em que o endereço IP de origem pertence a outra pessoa, o proprietário do endereço tem de remover o bloqueio do site Spamhaus. Se o endereço IP estiver na Lista de Bloqueios de Política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remover o endereço da PBL.

- No caso de mensagens de saída do seu domínio bloqueadas ligadas à Microsoft, pode receber este erro se as mensagens são encamistadas através de um serviço de terceiros. Pode utilizar uma ferramenta de procura WHOIS para encontrar o proprietário do endereço IP bloqueado.
