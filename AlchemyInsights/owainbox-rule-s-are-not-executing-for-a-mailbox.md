---
title: 1332 OWA - As regras da caixa de entrada não estão a ser executadas para uma caixa de correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576571"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Uma regra da caixa de entrada não funciona como esperado

Verifique as seguintes definições no Outlook na web:

- Uma mensagem pode ser redirecionada, reencaminhada ou respondeu automaticamente com base nas regras da Caixa de Entrada apenas uma vez. Uma regra de redirecionamento (regra de entrada ou fluxo de correio, também conhecida como regra de transporte) pode adicionar um máximo de dez destinatários de encaminhamento a uma mensagem. Para obter mais informações, consulte [os limites das regras journal, transport e inbox](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- As regras da caixa de entrada não funcionam na caixa de correio de diário suplente. Para obter mais informações sobre a caixa de correio de diário alternativo, consulte [a caixa de correio de diário suplente](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Para corrigir estas questões, consulte [o KB 2829319](https://support.microsoft.com/kb/2829319).

Se os problemas anteriores não se aplicarem, execute o relatório de diagnóstico da regra da caixa de entrada antes de aumentar o problema para o Microsoft Support:

1. Abra a caixa de correio no Outlook na web e clique em <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Configurações**  >  **Ver todas as Definições de Outlook**  >  **Correio**  >  **Regras.**

2. Na parte inferior da página, clique se **as suas regras não estiverem a funcionar clique aqui para gerar um relatório de diagnóstico**.
