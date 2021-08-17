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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117099"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge

Microsoft Edge problemas [conhecidos que](https://go.microsoft.com/fwlink/?linkid=2140608) estão relacionados com as zonas de segurança e podem afetar a forma como os utilizadores do Azure iniciarem sessão no Windows de Administração. Se estiver a ter problemas ao utilizar funcionalidades do Azure com o Microsoft Edge, experimente os seguintes passos:

1. No menu **Iniciar,** procure Opções da **Internet e selecione-as.**
2. Na caixa **de diálogo Propriedades** da Internet, vá para o **separador** Segurança.
3. Selecione **a zona Sites fided** fundo e, em seguida, selecione **o botão** Sites.
4. Na caixa de diálogo Sites fideditas, adicione o URL do seu gateway e, em  [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) seguida, selecione **Fechar**.
5. Na caixa **de diálogo Propriedades** da Internet, vá para o **separador** Privacidade.
6. Na secção **Bloqueador de Pop-up,** selecione **Definições**. Na caixa de diálogo que é aberta, adicione o URL do seu gateway e, em [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) seguida, selecione **Fechar**.
