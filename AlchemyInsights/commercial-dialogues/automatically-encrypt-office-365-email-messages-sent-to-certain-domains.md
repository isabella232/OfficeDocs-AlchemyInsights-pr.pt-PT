---
title: Encriptar automaticamente Office 365 e-mails enviados para determinados domínios
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082197"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Encriptar automaticamente Office 365 e-mails enviados para determinados domínios

1. No centro [de Exchange , selecionar](https://outlook.office365.com/ecp/)regras de fluxo de **> correio**. 
2. Clique no **ícone Novo (+)** e, em seguida, clique em **Aplicar Encriptação de Mensagens do Office 365 proteção de direitos e direitos a mensagens**.
3. Em **Nome**, introduza um nome para a regra, como *Encriptar mensagens enviadas para o contoso.com*.
4. Em **Aplicar esta regra se**, selecionar O destinatário > domínio **é**. 
5. Introduza o nome do domínio, por **exemplo, contoso.com**.
6. Clique no **ícone Adicionar (+)** e, em seguida, clique **em OK.**
7. Junto ao campo **Faça o seguinte,** clique em **Selecionar um**. 
8. No menu **superior do modelo RMS,** selecione Encriptar **e,** em seguida, clique **em OK.** (Se não vir esta opção, significa que o seu plano não inclui encriptação automática. Mas pode adicioná-lo!)
9. Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer nesta fase, muitas das quais podem ser deixadas com a predefinição para simplificação).
10. Clique em **Guardar**.

> [!IMPORTANT]
> Pode sempre voltar e editar esta regra mais tarde.

Para obter mais informações sobre como criar regras para encriptação, consulte Definir regras de fluxo de correio para encriptar mensagens de [e-mail Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)