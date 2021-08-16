---
title: Corrigir as definições da política de utilizador/caixa de correio
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034729"
---
# <a name="fix-user-policymailbox-settings"></a>Corrigir as definições da política de utilizador/caixa de correio

As definições de e-mail de lixo na caixa de correio afetaram esta mensagem. Para rever as definições, faça o seguinte:

1. Inceda Exchange Shell de Gestão. Para obter mais informações, consulte [Abrir a Shell Exchange Gestão de Dados](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Execute este comando (utilizando o endereço de e-mail do utilizador):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Verifique se o endereço de e-mail do remetente faz parte de **TrustedSendersAndDomains** ou **BlockedSendersAndDomains.** Se o endereço de e-mail estiver numa das listas, poderá ter de o remover. Para saber mais, consulte [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
