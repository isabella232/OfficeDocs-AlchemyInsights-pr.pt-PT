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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988217"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saiba quem configura o re encaminhamento numa caixa de correio e como

Se o re encaminhamento externo tiver sido definido numa caixa de correio, a atividade é auditada como parte do cmdlet Set-Mailbox correio. Eis como encontrar a atividade no registo de auditoria:

1. Vá para o Centro [de conformidade Office 365 de & de Conformidade.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. **Selecione** >  **Pesquisar registo de auditoria .**
    > [!NOTE]
    > Se vir um aviso a dizer que precisa de a ligar a auditoria, continue e a ligue-o agora. Se esta funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.
1. Certifique-se **de que o campo** Atividades está definido para Mostrar resultados para todas as atividades **(a predefinição).** Especifique o intervalo de datas. Não precisa de especificar um nome de utilizador.
1. **Selecione Procurar**. As atividades são apresentadas em **Resultados.**
1. **Selecione Filtrar** Resultados e, em **seguida, introduza Definir caixa de** correio no campo **de** filtro Atividade. Esta ação devolve todas **as atividades de Set-Mailbox.**
1. Para ver os detalhes, selecione uma atividade e, em seguida, **selecione Mais Informações.** Em **Parâmetros,** pode ver o endereço de e-mail de remetente que foi definido na caixa de correio. O **UserID** representa o utilizador que configura o rediamento externo na caixa de correio.
Para saber mais, consulte [Procurar no registo Office 365 auditoria de pesquisa para remoção de cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)