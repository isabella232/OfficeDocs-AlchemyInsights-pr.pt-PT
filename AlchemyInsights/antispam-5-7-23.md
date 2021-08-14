---
title: Antisspam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932180"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrigir problemas de entrega de e-mail com o código de erro 5.7.23

Verifique o registo DNS SPF do seu domínio num verificador de registos SPF ou DNS disponível publicamente na Web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encamilhada através do Grupo de Entrega de [Alto Risco.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) As mensagens no Grupo de Entrega de Alto Risco não passam verificações SPF, pelo que não serão aceites pela organização do e-mail de destino.

Se o problema persistir, poderá ter de contactar o administrador do anfitrião de correio para o qual está a tentar enviar e-mails. Anote o erro externo detalhado disponível na mensagem de resgate. O suporte da Microsoft poderá não conseguir ajudar mais.
