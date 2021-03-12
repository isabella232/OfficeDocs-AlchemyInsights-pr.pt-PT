---
title: Criptografe automaticamente certas mensagens de correio e-mail do escritório 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749460"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Criptografe automaticamente certas mensagens de correio e-mail do escritório 365

1. A partir do [centro de administração Exchange,](https://outlook.office365.com/ecp/)escolha **o fluxo de correio > regras**. 
2. Clique no ícone **Novo (+)** e, em seguida, clique **em Aplicar A encriptação de mensagens 365 e proteção de direitos para mensagens**.
3. Em **Nome**, introduza um nome para a regra, como *encriptar todas as mensagens*.
4. Em **Aplicar esta regra se,** escolher **[Aplicar a todas as mensagens]**. 
5. Ao lado do campo **Fazer o seguinte,** clique **em Selecionar um**. 
6. No menu drop-down **do modelo RMS,** selecione **Encrypt** e, em seguida, clique **em OK**. (Se não vir esta opção, significa que o seu plano não inclui encriptação automática. Mas pode adicioná-lo!)
7. Verifique a Auditoria esta regra com caixa **de verificação de nível de severidade** e, em seguida, selecione o nível pretendido. Se a sua empresa tiver obrigações contratuais para enviar todos os e-mails encriptados, recomendo definir o nível para **High**.
8. Em **Escolha um modelo para esta regra,** clique em **Enforce**. 
9. Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer neste momento, muitas das quais podem ficar com a definição padrão para a simplicidade).
10. Clique em **Guardar**.

> [!IMPORTANT]
> Pode sempre voltar e editar esta regra mais tarde.

Para obter mais informações sobre a criação de regras para encriptação, consulte [Regras de fluxo de correio para encriptar mensagens de correio eletrónico no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

