---
title: O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812875"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge

Microsoft Edge problemas conhecidos relacionados com zonas de segurança que podem afetar a forma como os utilizadores do Azure iniciarem sessão no Windows de administração. Para obter mais informações, consulte [Problemas conhecidos no Edge.](https://go.microsoft.com/fwlink/?linkid=2140608) Se estiver a ter problemas em utilizar funcionalidades do Azure com o Microsoft Edge, experimente o seguinte:

1. No menu Iniciar, na barra Procurar, **escreva** Opções da **Internet** e, em seguida, selecione-as.
1. Em **Propriedades da Internet**, selecione o **separador** Segurança.
1. **Selecione Sites Fided fundo e,** em seguida, **selecione Sites**.
1. Adicione o URL do seu gateway, bem como <https://login.microsoftonline.com> e <https://login.live.com> selecione **Fechar**.
1. Em **Propriedades da Internet**, selecione o **separador** Privacidade.
1. Na secção Bloqueador de Pop-up, selecione **Definições**. Adicione o URL do gateway, bem como e <https://login.microsoftonline.com> <https://login.live.com> e, em seguida, **selecione Fechar.**