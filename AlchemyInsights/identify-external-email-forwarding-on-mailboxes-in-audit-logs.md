---
title: Identificar o re encaminhamento de e-mails externos em caixas de correio em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630260"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o re encaminhamento de e-mail externo está configurado em caixas de correio

Quando um Microsoft 365 configura o encaminhamento de e-mail externo numa caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox.** Pode ver a atividade através da pesquisa de registo de auditoria no Centro de conformidade & segurança.

1. In iniciar sessão no [Centro Microsoft 365 conformidade.](https://protection.office.com/)

2. Aceda à página **Pesquisa de registo** de auditoria  >  **de** pesquisa.

3. Selecione o intervalo de **datas nos campos Data de início** e Data **de** fim. Não precisa de especificar um nome de utilizador. Verifique se o **campo Atividades** está definido para Mostrar resultados de todas **as atividades.**

4. Clique **em Procurar**.

Nos resultados, clique em **Filtrar Resultados** e escreva **Definir Caixa de Correio** na caixa de filtro de atividade. Selecione um registo de auditoria nos resultados. Na **panfleto** Detalhes, clique **em Mais informações.** Tem de ver os detalhes de cada registo de auditoria para determinar se a atividade está relacionada com o re encaminhamento de e-mails.

- **ObjectId:** o valor do alias da caixa de correio que foi modificada.

- **Parâmetros:** _ForwardingSmtpAddress indica_ o endereço de e-mail de destino.

- **UserId:** o utilizador que configurou o re encaminhamento de e-mail na caixa de correio no **campo ObjectId.**

Para obter mais informações, consulte Determinar [quem configurar o receção de e-mails para uma caixa de correio.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
