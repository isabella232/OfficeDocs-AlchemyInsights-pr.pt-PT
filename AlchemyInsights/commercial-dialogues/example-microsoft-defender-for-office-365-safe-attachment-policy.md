---
title: Exemplo do Microsoft Defender para Office 365 Cofre Anexos
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988306"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exemplo do Microsoft Defender para Office 365 Cofre Anexos

Estas definições ativam uma política denominada Sem *atrasos* que entrega mensagens imediatamente e, em seguida, volta a ajustar os anexos após a análise:

- **Nome:** Sem atrasos
- **Descrição:** fornece mensagens imediatamente e volta a aninhar os anexos após a análise.
- **Resposta:** selecione **a opção Entrega Dinâmica.** Para obter mais informações, consulte [Entrega Dinâmica Cofre políticas de Anexos.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Redirecionar** a secção de anexos: selecione a opção para Ativar **o redirecionamento** e, em seguida, introduza o endereço de e-mail do seu administrador global, administrador de segurança ou analista de segurança do Microsoft 365 que irá investigar anexos maliciosos.
- **Aplicado A secção: Selecione** O **domínio do destinatário é e, em** seguida, selecione o seu domínio. **Selecione adicionar** e, em seguida, **selecione OK.** Quando terminar, selecione **Guardar**.

Para saber mais, consulte [o Cofre Anexos no Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
