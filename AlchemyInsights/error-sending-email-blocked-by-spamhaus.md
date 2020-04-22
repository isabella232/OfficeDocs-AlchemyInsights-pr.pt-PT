---
title: Envio de erro de e-mail bloqueado por SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714269"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Envio de erro: Anfitrião do cliente bloqueado usando Spamhaus

O endereço IP que enviou a mensagem está numa lista de blocos propriedade da [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). As razões para ser bloqueado pela Spamhaus incluem contas comprometidas, máquinas comprometidas que partilham um endereço IP público e políticas de Fornecedor de Serviços de Internet (ISP). As possíveis correções são:
  
- Para mensagens de entrada bloqueadas onde controla o servidor de e-mail fonte, é necessário determinar a causa e remover o bloco do website spamhaus.

- Para mensagens de entrada bloqueadas onde o endereço IP de origem pertence a outra pessoa, o proprietário do endereço precisa remover o bloco do site Spamhaus. Se o endereço IP estiver na Lista de Blocos de Política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remover o endereço do PBL.

- Para mensagens de saída bloqueadas do seu domínio ligados à Microsoft, pode receber este erro se as mensagens forem encaminhadas através de um serviço de terceiros. Você pode usar uma ferramenta de procuração WHOIS para encontrar o proprietário de endereço IP bloqueado.
