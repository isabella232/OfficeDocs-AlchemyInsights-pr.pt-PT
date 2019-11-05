---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964267"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corrigir problemas de entrega para código de erro 550 5.4.1 Acesso ao relé negado

Esse problema ocorre ao verificar se um endereço de [e-mail é válido para evitar retornos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede Office 365. Experimente o seguinte:

1. Determine se o problema é específico para um domínio inteiro ou um único endereço de e-mail:
    - Domínio inteiro: Às vezes o domínio precisa ser sincronizado; tentar [definir o domínio para interno e, em seguida, de volta ao Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Endereço de e-mail único: Às vezes, o endereço precisa ser sincronizado; mudar o endereço de proxy smtp e, em seguida, alcomodá-lo de volta pode ajudar.
2. Determine se o problema é específico para um grupo ou pasta pública. Para alguns tipos de objetos, os objetos podem precisar ser criados manualmente no Diretório Ativo Do Azure.

Se você precisar de ajuda adicional, abra um bilhete de suporte e especifique o escopo do problema (incluta o tipo de objeto para o qual você está enviando) para que possamos ajudá-lo melhor.