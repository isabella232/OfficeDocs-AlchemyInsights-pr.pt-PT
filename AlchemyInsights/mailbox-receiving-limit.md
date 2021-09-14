---
title: A receção de caixas de correio limita a imposição
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316038"
---
# <a name="mailbox-receiving-limit-enforcement"></a>A receção de caixas de correio limita a imposição

A Microsoft começou recentemente a impor o limiar por caixa de correio de 3600 mensagens por hora. Para obter mais informações, [consulte limites Exchange Online de utilização.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 caixas de correio que recebem mais de 3600 mensagens no espaço de uma hora são cronáveis para os próximos 60 minutos. 

Além disso, é aplicado o limite de pares de remetente-destinatário (SRP) que bloqueia as mensagens recebidas por uma caixa de correio Microsoft 365 de um remetente específico. Se um único remetente enviar mais de 33% do limiar total ou de 1200 mensagens por hora a um destinatário específico, o limite SRP é ativado e a caixa de correio deixa de aceitar mensagens do remetente em questão. Tenha em atenção que:

- Este limite é uma aplicação para e-mails recebidos de outros inquilinos, no local ou de re talões de Internet.
- A entrega de e-mail na caixa de correio é bloqueada durante os próximos 60 minutos. 
- Os remetidos para estas caixas de correio recebem um relatório de entrega sem data de entrega (5.2.121 ou 5.2.122) a indicar que a caixa de correio excedeu o limiar de entrega máximo. O inquilino intra-inquilino (correio no mesmo inquilino) continua a ser entregue.
- Quando o limite SRP é aplicado, a caixa de correio de receção continuará a aceitar mensagens de outros recetores.

Os administradores podem monitorizar a atividade atual da caixa de correio ao aceder a um novo relatório e ao dados no centro de administração do Exchange denominado "Caixas de correio que excedem os limites de receção". As inquilinos só aparecem se um inquilino ofender as caixas de correio, enquanto o relatório aparece sempre no dashboard mas está vazio, a menos que um inquilino tenha ofensivo caixas de correio.

Para obter mais informações sobre limites de receção de informações, consulte o artigo Caixas de correio que excedem os limites de receção de informações [no novo EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Para obter mais informações sobre o relatório de limites de receção excedido, consulte o artigo Caixas de correio que excedem o relatório de limites de receção [no novo EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)