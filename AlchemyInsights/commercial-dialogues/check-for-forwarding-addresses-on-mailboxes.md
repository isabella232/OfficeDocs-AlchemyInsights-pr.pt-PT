---
title: Verificar se os endereços de re encaminhamento são enviados em caixas de correio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: a67305ed92e181f0ddfc5a929e8fe9631ceefdc99dea34118bc99975461f3868
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005821"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a>Verificar se os endereços de re encaminhamento são enviados em caixas de correio

Por vezes, os hackers reagem as mensagens de e-mail dos utilizadores para si próprios, pelo que, em primeiro lugar, iremos verificar se existem endereços e regras de re encaminhamento na caixa de correio. Em seguida, iremos verificar os registos de auditoria. Eis como verificar a procura de endereços de re encaminhamento:

1. **Selecione Utilizadores**  >  **Ativos.**
1. Selecione o utilizador cuja conta foi comprometida.
1. Na lista de listas que é exibida, expanda **Lista de Definições** e, em seguida, clique em **Editar para** Recaminhamento de **e-mail**.
1. Remova quaisquer endereços de re encaminhamento que não reconheça.