---
title: Nenhuma subscrição encontrada mensagem no Centro de Segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713962"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Nenhuma subscrição encontrada mensagem no Centro de Segurança

Se ao aceder ao Microsoft Defender Security Center obtém uma mensagem "Sem subscrições encontradas", significa que o Azure Ative Directory (AAD) utilizado para iniciar sessão no portal não tem uma licença ATP do Microsoft Defender.  

As licenças Windows E5 e Office E5 são licenças separadas.

Abra um caso de apoio se a licença foi comprada mas não for provisionada a este caso AAD. Ou tem: <br/>
-   Um possível problema de provisionamento de licença.<br/>
-   Inadvertidamente, ademticou a licença a um Microsoft AAD diferente daquele utilizado para autenticação no serviço.