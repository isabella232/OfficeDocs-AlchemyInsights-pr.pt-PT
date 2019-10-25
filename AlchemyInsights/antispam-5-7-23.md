---
title: Antispam - 5,7,23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682246"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corrigir problemas de entrega de e-mail para código de erro 5.7.23

Verifique o registro SPF DNS para o seu domínio em um verificador de registro SPF ou DNS disponível publicamente na web.

Verifique se a mensagem de saída não foi identificada como spam pelo Office 365 e encaminhada através do Pool de Entrega de [Alto Risco.](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages) As mensagens no Pool de Entrega de Alto Risco não passarão nas verificações do FPS e, portanto, não serão aceitas pela organização de e-mail de destino.

Se o problema persistir, você pode precisar entrar em contato com o administrador do mail host para o qual você está tentando enviar e-mail. Anote o erro externo detalhado disponível na mensagem de rejeição.  O suporte do Escritório 365 pode não ser capaz de ajudar ainda mais.