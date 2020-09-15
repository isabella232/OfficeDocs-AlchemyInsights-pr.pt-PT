---
title: Anti-paspam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717336"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrija os problemas de entrega de e-mail para código de erro 5.7.23

Verifique o registo de DNS SPF para o seu domínio num verificador de registo SPF ou DNS disponível publicamente na web.

Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do [Pool de Entrega de Alto Risco](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). As mensagens no Pool de Entrega de Alto Risco não passarão cheques SPF, pelo que não serão aceites pela organização de email de destino.

Se o problema persistir, poderá ter de contactar o administrador do anfitrião do correio para o qual está a tentar enviar e-mail. Tome nota do erro externo detalhado disponível na mensagem de ressalto. O suporte da Microsoft pode não ser capaz de ajudar mais.
