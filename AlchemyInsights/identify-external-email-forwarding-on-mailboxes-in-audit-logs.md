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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539112"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o reencaminhamento de correio electrónico externo está configurado nas caixas de correio

Quando um utilizador do Office 365 configura o reencaminhamento de correio electrónico externo numa caixa de correio, a actividade é auditada como parte do cmdlet **Set-Mailbox** . Pode ver a actividade de utilizar a procura de registo de auditoria no & Security Center de conformidade.

1. Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/).

2. Vá para a **pesquisa**de > página de**procura de registo de auditoria** .

3. Seleccione o intervalo de datas nos campos **data de início** e **data de fim** . Não é necessário especificar um nome de utilizador. Verifique se que o campo de **actividades** é definido para **Mostrar resultados para todas as actividades**.

4. Clique em **Procurar**.

Nos resultados, clique em **Resultados de filtro** e escreva **Set-Mailbox** na caixa de actividade de filtragem. Seleccione um registo de auditoria nos resultados. Na lista de opções de **Detalhes** , clique em **obter mais informações**. Devem observar os detalhes de cada registo de auditoria para determinar se a actividade está relacionada para reencaminhamento de correio electrónico.

- **ObjectId**: O valor de alias da caixa de correio que foi modificado.

- **Parâmetros**: _ForwardingSmtpAddress_ indica o endereço de correio electrónico de destino.

- **ID de utilizador**: O utilizador configurado reencaminhamento de correio electrónico na caixa de correio no campo **ID de objecto** .

Para mais informações, consulte [determinar que configurou para uma caixa de correio de reencaminhamento de correio electrónico](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
