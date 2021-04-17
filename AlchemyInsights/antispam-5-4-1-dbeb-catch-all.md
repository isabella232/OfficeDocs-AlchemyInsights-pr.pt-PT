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
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821458"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corrigir problemas de entrega para código de erro 550 5.4.1 Relé De acesso negado

Este problema ocorre [ao verificar se um endereço de e-mail é válido para evitar retornos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede microsoft. Experimente o seguinte:

1. Determinar se o problema é específico de todo um domínio ou de um único endereço de e-mail:
    - Domínio inteiro: Por vezes, o domínio precisa de ser sincronizado; tente [definir o domínio para Interno e, em seguida, de volta para Autoritário](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Endereço de e-mail único: Por vezes, o endereço precisa de ser sincronizado; mudar o endereço de procuração smtp e, em seguida, mudá-lo de volta pode ajudar.
2. Determinar se o problema é específico de um grupo ou de uma pasta pública. Para alguns tipos de objetos, os objetos podem ter de ser criados manualmente no Diretório Ativo Azure.

Se precisar de ajuda adicional, abra um bilhete de apoio e especifique o âmbito do problema (incluindo o tipo de objeto que está a enviar) para que possamos ajudá-lo melhor.