---
title: O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583786"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge

O Microsoft Edge [tem conhecido problemas relacionados](https://go.microsoft.com/fwlink/?linkid=2140608) com zonas de segurança e pode afetar a forma como os utilizadores do Azure entram no Windows Admin Center. Se tiver problemas em utilizar funcionalidades do Azure com o Microsoft Edge, experimente os seguintes passos:

1. No menu **Iniciar,** procure **opções de Internet** e selecione-as.
2. Na caixa de diálogo **Internet Properties,** aceda ao **separador Segurança.**
3. Selecione a zona **de sites Fidedignos** e, em seguida, selecione o botão **'Sites'.**
4. Na caixa de diálogo **dos sites Fidedignos,** adicione o URL do gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e , [https://login.live.com](https://login.live.com) e, em seguida, selecione **Close**.
5. Na caixa de diálogo **Internet Properties,** aceda ao **separador Privacidade.**
6. Na secção **'Bloqueador Pop-up',** selecione **Definições**. Na caixa de diálogo que se abre, adicione o URL do gateway bem como [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) e , e, em seguida, selecione **Close**.
