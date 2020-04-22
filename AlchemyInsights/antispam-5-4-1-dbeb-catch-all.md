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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707922"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corrigir problemas de entrega para código de erro 550 5.4.1 Acesso de retransmissão negado

Este problema ocorre ao verificar se um endereço de [e-mail é válido para evitar ressaltos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft. Tente o seguinte:

1. Determine se o problema é específico de um domínio inteiro ou de um único endereço de e-mail:
    - Domínio inteiro: Às vezes o domínio precisa de ser sincronizado; tente [definir o domínio para Interno e, em seguida, de volta ao Authoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Endereço de e-mail único: Às vezes, o endereço precisa de ser sincronizado; mudar o endereço de procuração smtp e, em seguida, mudá-lo de volta pode ajudar.
2. Determine se o problema é específico de um grupo ou pasta pública. Para alguns tipos de objetos, os objetos podem ter de ser criados manualmente no Diretório Ativo Azure.

Se precisar de ajuda adicional, por favor abra um bilhete de apoio e especifique o âmbito do problema (incluindo o tipo de objeto que está a enviar) para que possamos ajudá-lo melhor.