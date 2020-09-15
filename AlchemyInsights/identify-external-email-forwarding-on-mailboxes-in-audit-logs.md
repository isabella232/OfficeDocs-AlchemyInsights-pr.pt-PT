---
title: Identificar reencaminhamento de e-mail externo em caixas de correio em registos de auditoria
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696308"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifique quando o reencaminhamento de e-mail externo é configurado em caixas de correio

Quando um utilizador do Microsoft 365 configura o envio de e-mails externos numa caixa de correio, a atividade é auditada como parte do **cmdlet Set-Mailbox.** Pode ver a atividade utilizando a pesquisa de registo de auditoria no Centro de Conformidade & de Segurança.

1. Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Aceda à página de pesquisa de registo de registo de auditoria **de pesquisa.**  >  **Audit log search**

3. Selecione o intervalo de datas nos campos **data de início** e **fim.** Não precisa de especificar um nome de utilizador. Verifique se o campo **de Atividades** está definido para **mostrar resultados para todas as atividades**.

4. Clique **em Pesquisar**.

Nos resultados, clique em **Resultados do Filtro** e escreva **Set-Mailbox** na caixa de filtro de atividade. Selecione um registo de auditoria nos resultados. No flyout **Details,** clique **em Mais informações.** Você tem que olhar para os detalhes de cada registo de auditoria para determinar se a atividade está relacionada com o reencaminhamento de e-mail.

- **ObjectId**: O valor do pseudónimo da caixa de correio que foi modificada.

- **Parâmetros**: _ReencaminhamentoSmtpAddress_ indica o endereço de e-mail-alvo.

- **UserId**: O utilizador que configura o reencaminhamento de e-mail na caixa de correio no campo **ObjectId.**

Para obter mais informações, consulte [Determineing quem criou o reencaminhamento de e-mail para uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
