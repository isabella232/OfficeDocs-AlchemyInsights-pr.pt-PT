---
title: Corrigir política de ligação
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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988135"
---
# <a name="fix-connection-policy"></a>Corrigir política de ligação

O e-mail foi marcado como seguro e entregue na caixa de entrada do utilizador porque o endereço IP de envio foi marcado como seguro na política Filtro de Ligação. Para rever a política, faça o seguinte:

1. Vá para o Centro [Office 365 de Conformidade &](https://go.microsoft.com/fwlink/p/?linkid=2077143)de Conformidade e, em seguida, vá para Política de Gestão de ameaças  >    >  [Antisspam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. No separador **Personalizar,** selecione a Política **de filtro de ligação e, em** seguida, selecione **Editar política.**
3. Reveja **a lista de Endereços IP** Permitidos. Veja se **a Cofre de lista está** ativada.

    > [!NOTE]
    > A Microsoft subscreve as fontes de terceiros de relevos de confiança. Se **Cofre lista de correio** estiver ativada, estes remetidos de confiança não são marcados por engano como spam. Recomendamos que selecione esta opção, pois reduzirá o número de falsos positivos (e-mails válidos classificados como spam) que recebe.
