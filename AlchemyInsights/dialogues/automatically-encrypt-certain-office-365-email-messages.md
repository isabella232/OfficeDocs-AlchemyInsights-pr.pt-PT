---
title: Criptografe automaticamente certas mensagens de correio-mail do Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526738"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Criptografe automaticamente certas mensagens de correio-mail do Office 365

Pode encriptar automaticamente as mensagens que os utilizadores enviam a determinadas pessoas ou organizações externas. Para isso, execute os seguintes passos:

1. A partir do [centro de administração Exchange,](https://outlook.office365.com/ecp/)escolha **o fluxo de correio > regras**. 
2. Clique no ícone **Novo (+)** e, em seguida, clique **em Aplicar A encriptação de mensagens 365 e proteção de direitos para mensagens**.
3. Em **Nome**, introduza um nome para a regra, como *mensagens encriptadas enviadas para DrToniRamos@gmail.com*.
4. Em **Aplicar esta regra se**, escolher o destinatário > é esta **pessoa**. 
5. Na janela **'Selecionar membros',** selecione o nome da pessoa a quem deseja que a regra de encriptação se aplique e, em seguida, clique em **adicionar**. 
6. Quando terminar de adicionar utilizadores, clique **em OK**.
7. Ao lado do campo **Fazer o seguinte,** clique **em Selecionar um**. 
8. No menu drop-down **do modelo RMS,** selecione **Encrypt** e, em seguida, clique **em OK**. (Se não vir esta opção, significa que o seu plano não inclui encriptação automática. Mas pode adicioná-lo!)
9. Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer neste momento, muitas das quais podem ficar com a definição padrão para a simplicidade).
10. Clique em **Guardar**.

> [!IMPORTANT]
> Pode sempre voltar e editar esta regra mais tarde.

Para obter mais informações sobre a criação de regras para encriptação, consulte [regras de fluxo de correio para encriptar mensagens de correio eletrónico no Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

