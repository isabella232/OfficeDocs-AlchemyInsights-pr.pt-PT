---
title: Identificar o reencaminhamento de correio electrónico externo nas caixas de correio nos registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383108"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o reencaminhamento de correio electrónico externo está configurado nas caixas de correio

Quando um utilizador configura o reencaminhamento de correio electrónico externo numa caixa de correio, a actividade é auditada como parte do cmdlet **Set-Mailbox** . Pode ver a actividade de utilizar a procura de registo de auditoria no & Security Center de conformidade.

1. Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/)

2. Clique em **Procurar e de investigação** e seleccione a **Procura de registo de auditoria**.

3. Seleccione o intervalo de datas nos campos **data de início** e **data de fim** . Não é necessário especificar um nome de utilizador. Verifique se que o campo de **actividades** é definido para **Mostrar resultados para todas as actividades**.

4. Clique em **Procurar**.

Nos resultados, clique em **Resultados de filtro** e escreva **Set-Mailbox** na caixa de actividade de filtragem. Seleccione um registo de auditoria nos resultados. Na lista de opções de **Detalhes** , clique em **obter mais informações**. Devem observar os detalhes de cada registo de auditoria para determinar se a actividade está relacionada para reencaminhamento de correio electrónico.

- **ObjectId**: O valor de alias da caixa de correio que foi modificado.

- **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de correio electrónico de destino.

- **ID de utilizador**: O utilizador configurado reencaminhamento de correio electrónico na caixa de correio no campo **ID de objecto** .

Para mais informações, consulte [determinar que configurou para uma caixa de correio de reencaminhamento de correio electrónico](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
