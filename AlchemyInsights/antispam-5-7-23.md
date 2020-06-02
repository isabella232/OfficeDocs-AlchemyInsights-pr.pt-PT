---
title: Anti-paspam - 5.7.23
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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506454"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrija os problemas de entrega de e-mail para código de erro 5.7.23

Verifique o registo de DNS SPF para o seu domínio num verificador de registo SPF ou DNS disponível publicamente na web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do [Pool de Entrega de Alto Risco](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). As mensagens no Pool de Entrega de Alto Risco não passarão cheques SPF, pelo que não serão aceites pela organização de email de destino.

Se o problema persistir, poderá ter de contactar o administrador do anfitrião do correio para o qual está a tentar enviar e-mail. Tome nota do erro externo detalhado disponível na mensagem de ressalto. O suporte da Microsoft pode não ser capaz de ajudar mais.
