---
title: Encontre o endereço IP no registo de auditoria
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429787"
---
# <a name="find-the-ip-address-in-audit-log"></a>Encontre o endereço IP no registo de auditoria

1. O endereço IP que corresponde a uma atividade realizada por um utilizador ou administrador é mostrado nos registos de auditoria. A informação do cliente também está registada. Aqui está como identificar o endereço IP:

1. Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione **pesquisa**  >  **[de registo de auditoria de pesquisa](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Se vir um aviso de que precisa de ligar a auditoria, vá em frente e ligue-o agora. Se esta funcionalidade não estiver ativada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.
1. Se estiver interessado numa atividade específica, selecione-a na lista **de Atividades;** caso contrário, por padrão, todas as atividades serão devolvidas para o utilizador selecionado. Note que certas atividades podem não estar disponíveis para seleção a partir do menu **Atividades;** no entanto, esses itens de auditoria serão devolvidos se **os resultados do Show para todas as atividades** forem selecionados (definição predefinida).
1. Especifique o intervalo de datas e, no campo **Utilizadores,** selecione o nome de utilizador para o utilizador que pretende investigar.
1. Selecione **Pesquisar**. As atividades aparecem nos **Resultados.** Pode ver o endereço IP de cada atividade.
1. Para ver detalhes, selecione uma atividade e, em seguida, selecione **Mais Informações**.

Para saber mais, consulte o [registo de auditoria do Office 365 para resolver cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)