---
title: Encriptar automaticamente determinadas mensagens de e-mail do Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988846"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Encriptar automaticamente determinadas mensagens de e-mail do Office 365

1. No centro [de Exchange , selecionar](https://outlook.office365.com/ecp/)regras de fluxo de **> correio**. 
2. Clique no **ícone Novo (+)** e, em seguida, clique em **Aplicar Encriptação de Mensagens do Office 365 proteção de direitos e direitos a mensagens**.
3. Em **Nome**, introduza um nome para a regra, como *Encriptar todas as mensagens.*
4. Em **Aplicar esta regra se**, **selecionar [Aplicar a todas as mensagens]**. 
5. Junto ao campo **Faça o seguinte,** clique em **Selecionar um**. 
6. No menu **superior do modelo RMS,** selecione Encriptar **e,** em seguida, clique **em OK.** (Se não vir esta opção, significa que o seu plano não inclui encriptação automática. Mas pode adicioná-lo!)
7. Selecione a **caixa de verificação Auditar esta regra com nível de** gravidade e, em seguida, selecione o nível pretendido. Se a sua empresa tiver obrigações contratuais para enviar todos os e-mails encriptados, recomendamos que desmarca o nível para **Alto.**
8. Em **Escolher um modelo para esta regra**, clique em **Impor**. 
9. Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer nesta fase, muitas das quais podem ser deixadas com a predefinição para simplificação).
10. Clique em **Guardar**.

> [!IMPORTANT]
> Pode sempre voltar e editar esta regra mais tarde.

Para obter mais informações sobre como criar regras para encriptação, consulte Definir regras de fluxo de correio para encriptar mensagens de [e-mail Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

