---
title: Descubra quem se instalou a encaminhar uma caixa de correio, e como
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429991"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Descubra quem se instalou a encaminhar uma caixa de correio, e como

Se o reencaminhamento externo foi colocado numa caixa de correio, a atividade é auditada como parte do Set-Mailbox cmdlet. Eis como encontrar a atividade no registo de auditoria:

1. Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **pesquisa** >  **de registo de auditoria de pesquisa**.
    > [!NOTE]
    > Se vir um aviso de que precisa de ligar a auditoria, vá em frente e ligue-o agora. Se esta funcionalidade não estiver ligada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.
1. Certifique-se de que o campo **Atividades** está definido para **mostrar resultados para todas as atividades** (o padrão). Especifique o intervalo de datas. Não precisa de especificar um nome de utilizador.
1. Selecione **Pesquisar**. As atividades aparecem nos **Resultados.**
1. Selecione **Resultados do Filtro** e, em seguida, **introduza a caixa de correio** de set no campo do filtro **Desemundo.** Isto devolve todas as atividades **da Set-Mailbox.**
1. Para ver os detalhes, selecione uma atividade e, em seguida, selecione **Mais Informações**. Em **Parâmetros** pode ver o endereço de e-mail de encaminhamento que foi definido na caixa de correio. O **UserID** representa o utilizador que configura o reencaminhamento externo na caixa de correio.
Para saber mais, consulte [o registo de auditoria do Office 365 para resolver cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)