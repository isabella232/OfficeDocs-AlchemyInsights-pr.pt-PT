---
title: Remoção de Eventos a partir de E-mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105363"
---
# <a name="troubleshooting-events-from-email"></a>Remoção de Eventos a partir de E-mail

1. Verificar se a funcionalidade está ativada para a caixa de correio: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Em seguida, veja os registos "Eventos de **E-mail" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Nos registos "Eventos a partir de E-mail", procure o IDDoMessageId da Internet que corresponde ao item na caixa de correio.  

4. O trustScore determina se o item é adicionado ou não. Os eventos só serão adicionados se o trustScore = "Trusted".

A pontuação TrustScore é determinada pelas propriedades SPF, Dkim ou Dmarc, que estão no Cabeçalho da Mensagem.

Para ver estas propriedades:

**Ambiente de Outlook**

- Abrir o item
- File -> Propriedades -> Cabeçalhos da Internet

ou

**MFCMapi**

- Navegar para o item na caixa de entrada
- Procure por PR_TRANSPORT_MESSAGE_HEADERS_W

Estas propriedades são determinadas e gravadas durante o transporte e o reencaminhamento. Para obter mais remoção de problemas, poderá ter de obter Suporte de Transporte sobre as falhas no SPF, DKIM e.ou DMARC.