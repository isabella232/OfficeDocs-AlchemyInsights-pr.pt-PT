---
title: Corrigir a política de ligação
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750604"
---
# <a name="fix-connection-policy"></a>Corrigir a política de ligação

O e-mail foi marcado como seguro e entregue na caixa de entrada do utilizador porque o endereço IP de envio estava marcado como seguro na política do Filtro de Ligação. Para rever a política, faça o seguinte:

1. Vá ao [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), e depois vá para a Política de **Gestão** de Ameaças  >    >  [Antisspam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. No separador **'Personalizado',** selecione a política do **filtro 'Ligação'** e, em seguida, selecione **a política de edição**.
3. Reveja a lista **de IP Allow.** Veja se **a lista Safe** está ativada.

    > [!NOTE]
    > A Microsoft subscreve fontes de emissores de confiança de terceiros. Se **a lista "Safe"** estiver ativada, estes remetentes fidedignos não são erroneamente marcados como correio publicitário não-correio eletrónico. Recomendo a seleção desta opção, pois reduzirá o número de falsos positivos (bom correio que é classificado como spam) que recebe.
