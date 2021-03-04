---
title: Verifique se há endereços de encaminhamento nas caixas de correio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427713"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Verifique se há endereços de encaminhamento nas caixas de correio

Por vezes, os hackers encaminham as mensagens de e-mail dos utilizadores para si mesmos, por isso, primeiro, vamos verificar se enviamos endereços e regras na caixa de correio. Depois vamos verificar os registos de auditoria. Aqui está como verificar se os endereços de encaminhamento:

1. Selecione **utilizadores**  >  **Utilizadores Ative**.
1. Selecione o utilizador cuja conta foi comprometida.
1. No flyout que aparece, expanda **as Definições de Correio** e, em seguida, clique em **Editar** para **reencaminhamento de e-mail**.
1. Remova quaisquer endereços de reencaminhamento que não reconheça.