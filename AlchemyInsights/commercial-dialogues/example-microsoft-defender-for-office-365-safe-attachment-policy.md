---
title: Exemplo Microsoft Defender para a política de anexo seguro do Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749200"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exemplo Microsoft Defender para a política de anexo seguro do Office 365

Estas definições permitem uma política chamada *Sem atrasos* que entregue mensagens imediatamente e depois reata os anexos após a sua digitalização:

- **Nome**: Sem atrasos
- **Descrição**: Entrega mensagens imediatamente e reacando os anexos após a digitalização.
- **Resposta**: Selecione a opção **Entrega Dinâmica.** Para obter mais informações, consulte [a Entrega Dinâmica nas políticas de Anexos Seguros.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Redirecione** a secção de anexo: Selecione a opção para ativar o **redirecionamento** e, em seguida, insira o endereço de e-mail do seu administrador global Microsoft 365, administrador de segurança ou analista de segurança que irá investigar anexos maliciosos.
- **Aplicado Para a** secção: Selecione **O domínio do destinatário é** e, em seguida, selecione o seu domínio. **Selecione adicionar**, e, em seguida, selecione **OK**. Uma vez terminado, **selecione Save**.

Para saber mais, consulte [Anexos Seguros no Microsoft Defender para o Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
