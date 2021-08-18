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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331170"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar quando o re encaminhamento de e-mail externo está configurado em caixas de correio

Quando um Microsoft 365 configura o respetivo encaminhamento de e-mail externo numa caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox.** Pode ver a atividade através da pesquisa do registo de auditoria. Eis como fazê-lo.

1. Eis um dos seguintes passos:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria de  \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://sip.security.microsoft.com/auditlogsearch> .

2. Na página **Auditoria,** verifique se o separador **Procurar está** selecionado e, em seguida, configure as seguintes definições:
   - Selecione o intervalo de data/hora nas **caixas** **Início e** Fim.
   - Verifique se **a caixa Atividades** contém Mostrar resultados de todas as **atividades.**

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria.

4. Nos resultados, clique em **Filtrar Resultados** e escreva **Definir Caixa de Correio** na caixa de filtro de atividade.

5. Selecione um registo de auditoria nos resultados. Na **panfleto** Detalhes, clique **em Mais informações.** Tem de ver os detalhes de cada registo de auditoria para determinar se a atividade está relacionada com o re encaminhamento de e-mails.

   - **ObjectId:** o valor do alias da caixa de correio que foi modificada.
   - **Parâmetros:** _ForwardingSmtpAddress indica_ o endereço de e-mail de destino.
   - **UserId:** o utilizador que configurou o re encaminhamento de e-mail na caixa de correio no **campo ObjectId.**

Para obter mais informações, consulte Determinar [quem configurar o receção de e-mails para uma caixa de correio.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
