---
title: Identificar o envio externo de e-mails nas caixas de correio em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716471"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifique quando o reencaminhamento externo de e-mails está configurado nas caixas de correio

Quando um utilizador da Microsoft 365 configura o envio de e-mail externo numa caixa de correio, a atividade é auditada como parte do cmdlet **set-mailbox.** Pode ver a atividade utilizando a pesquisa de registo de auditoria no Security & Compliance Center.

1. Inicie sessão no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Aceda à página de pesquisa de registo de auditoria de > **pesquisa.** **Search**

3. Selecione o intervalo de data sintetiza-se nos campos de data de **início** e data de **fim.** Não precisa especificar um nome de utilizador. Verifique se o campo **De atividades** está definido para **mostrar resultados para todas as atividades.**

4. Clique em **Procurar**.

Nos resultados, clique em **Resultados do Filtro** e digite **Set-Mailbox** na caixa de filtro de atividade. Selecione um registo de auditoria nos resultados. Nos **Detalhes,** clique em **Mais informações.** Você tem que olhar os detalhes de cada registo de auditoria para determinar se a atividade está relacionada com o reencaminhamento de e-mail.

- **ObjectId**: O valor do pseudónimo da caixa de correio que foi modificado.

- **Parâmetros**: _ReencaminhamentoSmtpAddress_ indica o endereço de e-mail alvo.

- **UserId**: O utilizador que configurao o envio de e-mail na caixa de correio no campo **ObjectId.**

Para mais informações, consulte [Determinar quem configura o envio de e-mail para uma caixa de correio](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
