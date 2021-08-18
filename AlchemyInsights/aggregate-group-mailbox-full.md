---
title: AgregateGroupMailbox full NDR recebido para e-mail enviado para Microsoft 365 grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315921"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AgregateGroupMailbox full NDR recebido para e-mail enviado para Microsoft 365 grupo

Utilize o seguinte comando Shell do EXO para criar uma regra de transporte Exchange para largar de forma automática os e-mails enviados para a caixa de correio de grupo agregada:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Nota:** substitua o endereço SMTP em **-SentTo** por endereço SMTP da caixa de correio de grupo agregada no seu inquilino. Pode obter o endereço SMTP da caixa de correio de grupo agregada a partir do NDR recebido.



