---
title: Corrigir as definições da política do utilizador/caixa de correio
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750559"
---
# <a name="fix-user-policymailbox-settings"></a>Corrigir as definições da política do utilizador/caixa de correio

As definições de correio publicitário não solicitado na caixa de correio afetaram esta mensagem. Para rever as definições, faça o seguinte:

1. Launch Exchange Management Shell. Para mais informações, consulte [Abrir a Shell de Gestão de Câmbios.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Executar este comando (utilizando o endereço de e-mail do utilizador):  **obter caixa de correio eletrónicoconfiguration -identidade "user@domain.com"**
3. Verifique se o endereço de e-mail do remetente faz parte de **TrustedSendersAndDomains** ou **BlockedSendersAndDomains**. Se o endereço de e-mail estiver numa das listas, poderá ter de o remover. Para saber mais, consulte [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
