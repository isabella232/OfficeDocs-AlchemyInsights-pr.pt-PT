---
title: Saiba quem configura o re encaminhamento numa caixa de correio e como
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895190"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saiba quem configura o re encaminhamento numa caixa de correio e como

Se o re encaminhamento externo tiver sido definido numa caixa de correio, a atividade é auditada como parte do cmdlet **Set-Mailbox.** Eis como encontrar a atividade no registo de auditoria:

1. Eis uma das seguintes ações:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria **de** \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Se vir um aviso a dizer que precisa de a ligar a auditoria, continue e a ligue-o agora. Se esta funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.

2. Na página **Auditoria,** verifique se o separador **Procurar está** selecionado e, em seguida, configure as seguintes definições:
   - Selecione o intervalo de data/hora nas **caixas** **Início e** Fim.
   - Verifique se **a caixa Atividades** contém Mostrar resultados de todas as **atividades.**

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria.

4. Nos resultados, clique na coluna **Atividade para** ordenar os resultados e procure **entradas de Definir Caixa de** Correio.

5. Selecione uma atividade nos resultados para abrir a panfleto de detalhes. Tem de ver os detalhes de cada registo de auditoria para determinar se a atividade está relacionada com o re encaminhamento de e-mails:
   - **ObjectId:** o valor do alias da caixa de correio que foi modificada.
   - **Parâmetros:** _ForwardingSmtpAddress indica_ o endereço de e-mail de destino.
   - **UserId:** o utilizador que configurou o re encaminhamento de e-mail na caixa de correio no **campo ObjectId.**

Para obter mais informações, consulte Determinar [quem configurar o receção de e-mails para uma caixa de correio.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
