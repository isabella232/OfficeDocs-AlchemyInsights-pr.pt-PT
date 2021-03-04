---
title: Leia os registos de auditoria para eventos apagados
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429826"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leia os registos de auditoria para eventos apagados

Eis como fazer isto:

1. Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **pesquisa**  >  [**de registo de auditoria de pesquisa**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Se vir um aviso de que precisa de ligar a funcionalidade, ligue-a agora. Se a funcionalidade não estiver ligada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.
1. Selecione **Atividades** e, em seguida, encontre **atividades de Caixa de Correio de Troca**. Selecione as **mensagens eliminadas da pasta de itens eliminados** e mude as mensagens para opções de pasta de **itens eliminados.** Quando terminar, clique fora do painel para minimizar o painel **de Atividades.**
1. Especifique o intervalo de datas e, em seguida, na caixa **Utilizadores,** selecione o nome de utilizador para o utilizador que pretende investigar. Pode selecionar mais do que um utilizador de cada vez.
1. Selecione **Pesquisar**. As atividades aparecem nos **Resultados.**
1. Para ver os detalhes, selecione uma atividade e, em seguida, selecione **Mais Informações**. Informações adicionais sobre o item eliminado, como a linha de assunto e a localização do item quando foi eliminado, são exibidas no campo **AffectedItems.**
    > [!NOTE]
    > Não é possível restaurar itens eliminados utilizando a função de registo de auditoria. Para restaurar os itens eliminados, consulte [Recuperar itens eliminados ou e-mail na App Outlook Web](https://go.microsoft.com/fwlink/?linkid=2103759).

Para saber mais, consulte [o registo de auditoria do Office 365 para resolver cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)
