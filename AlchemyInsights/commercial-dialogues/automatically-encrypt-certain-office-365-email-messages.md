---
title: Encriptar automaticamente determinadas mensagens Office 365 e-mail
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
ms.openlocfilehash: b15a72ced4921b3df1b7105837592781188a2a25
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327985"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Encriptar automaticamente determinadas mensagens Office 365 e-mail

Pode encriptar automaticamente as mensagens que os utilizadores enviam a determinadas pessoas ou organizações externas. Para o fazer, execute os seguintes passos:

1. No centro [de Exchange , selecionar](https://outlook.office365.com/ecp/)regras de fluxo de **> correio**. 
2. Clique no **ícone Novo (+)** e, em seguida, clique **em Aplicar Proteção Encriptação de Mensagens do Office 365 proteção de direitos a mensagens**.
3. Em **Nome**, introduza um nome para a regra, como *Encriptar mensagens enviadas para o DrToniRamos@gmail.com*.
4. Em **Aplicar esta regra se**, selecionar O destinatário > é esta **pessoa**. 
5. Na janela **Selecionar Membros,** selecione o nome da pessoa a quem pretende aplicar a regra de encriptação e, em seguida, clique em **adicionar**. 
6. Quando terminar de adicionar utilizadores, clique em **OK.**
7. Junto ao campo **Faça o seguinte,** clique em **Selecionar um**. 
8. No menu **superior do modelo RMS,** selecione Encriptar **e,** em seguida, clique **em OK.** (Se não vir esta opção, significa que o seu plano não inclui encriptação automática. Mas pode adicioná-lo!)
9. Escolha qualquer seleção opcional (a partir de uma lista de seleções opcionais que pode fazer nesta fase, muitas das quais podem ser deixadas com a predefinição para simplificação).
10. Clique em **Guardar**.

**Importante:** Pode sempre voltar e editar esta regra mais tarde.

Para obter mais informações sobre como criar regras para encriptação, consulte Definir regras de fluxo de correio para encriptar mensagens de [e-mail Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

