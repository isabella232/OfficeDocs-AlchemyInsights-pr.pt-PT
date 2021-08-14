---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932288"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corrigir problemas de entrega com o código de erro 550 5.4.1 Relay Access Denied

Este problema ocorre ao verificar se um endereço de e-mail é válido para impedir a [receção de comentários](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft. Experimente o seguinte:

1. Determine se o problema é específico de um domínio inteiro ou de um único endereço de e-mail:
    - Domínio completo: por vezes o domínio tem de ser sincronizado; tente [definir o domínio como Interno e, em seguida, volte a ser Autoritativo.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Endereço de e-mail único: por vezes, o endereço tem de ser sincronizado; alterar o endereço proxy smtp e, em seguida, recuá-lo pode ajudar.
2. Determine se o problema é específico de um grupo ou pasta pública. Para alguns tipos de objeto, os objetos podem ter de ser criados manualmente no Azure Active Directory.

Se precisar de ajuda adicional, abra um bilhete de suporte e especifique o âmbito do problema (incluindo o tipo de objeto para o qual está a enviar) para que o possamos ajudar melhor.