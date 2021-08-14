---
title: AgregarGroupMailbox full NDR recebido para e-mail enviado para Microsoft 365 grupo
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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951864"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AgregarGroupMailbox full NDR recebido para e-mail enviado para Microsoft 365 grupo

Utilize o seguinte comando Shell do EXO para criar uma regra de transporte Exchange para largar de forma automática os e-mails enviados para a caixa de correio de grupo agregada:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Substitua o endereço SMTP em **-SentTo** por endereço SMTP da caixa de correio de grupo agregada no seu inquilino. Pode obter o endereço SMTP da caixa de correio de grupo agregada a partir do NDR recebido.



