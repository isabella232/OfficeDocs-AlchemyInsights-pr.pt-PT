---
title: 1332 OWA – As regras de caixa de entrada não estão a ser executadas para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040913"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra de Caixa de Entrada não funciona conforme esperado

Verifique as seguintes definições no Outlook na Web:

- Uma mensagem só pode ser redirecionada, reencainhada ou respondida automaticamente com base nas regras da Caixa de Entrada uma única vez. Uma regra de redirecionamento (uma regra de Caixa de Entrada ou regra de fluxo de correio, também conhecida como regra de transporte) pode adicionar um máximo de dez destinatários de redireccionamento a uma mensagem. Para obter mais informações, consulte [Limites de regras de Diário,](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)Transporte e Caixa de Entrada.

- As regras de caixa de entrada não funcionam na caixa de correio de diário alternativa. Para obter mais informações sobre a caixa de correio de diário alternativa, consulte Caixa de [correio de diário alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Para corrigir estes problemas, consulte [o 2829319 .](https://support.microsoft.com/kb/2829319)

Se os problemas anteriores não se aplicarem, execute o relatório de diagnóstico da regra da Caixa de Entrada antes de escalar o problema para o Suporte da Microsoft:

1. Abra a caixa de correio no Outlook na Web e clique em <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Definições**  >  **Ver todas as Outlook Definições**  >  **Correio**  >  **Regras.**

2. Na parte inferior da página, clique em Se **as suas regras não estiverem a funcionar, clique aqui para gerar um relatório de diagnóstico**.
