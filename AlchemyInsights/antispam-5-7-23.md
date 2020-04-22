---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676508"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrija os problemas de entrega de e-mail para código de erro 5.7.23

Verifique o registo DoNs SPF para o seu domínio num verificador de registoS SPF ou DNS publicamente disponível na web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do Pool de Entrega de [Alto Risco](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). As mensagens no Pool de Entrega de Alto Risco não passarão em cheques SPF, pelo que não serão aceites pela organização de e-mails de destino.

Se o problema persistir, poderá ter de contactar o administrador do correio para o qual está a tentar enviar e-mail. Tome nota do erro externo detalhado disponível na mensagem de ressalta. O suporte da Microsoft pode não ser capaz de ajudar mais.
