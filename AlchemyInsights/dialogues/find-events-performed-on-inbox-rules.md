---
title: Encontrar eventos realizados nas regras da caixa de entrada
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430013"
---
# <a name="find-events-performed-on-inbox-rules"></a>Encontrar eventos realizados nas regras da caixa de entrada

Quando as regras da caixa de entrada são criadas, alteradas ou eliminadas, os eventos são registados no registo de auditoria. Eis como revê-los:

1. Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione Pesquisar > Audit pesquisa de registo.

    > [!NOTE]
    > Se vir um aviso de que precisa de ligar a auditoria, vá em frente e ligue-o agora. Se esta funcionalidade não estiver ligada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.
1. Selecione o campo Atividades e encontre as atividades da caixa de correio de Troca e, em seguida, selecione New-InboxRule Criar regra de caixa de entrada a partir da App Web do Outlook. Quando terminar, clique fora do painel para minimizar o painel de Atividades.
1. Especifique o intervalo de datas e, em seguida, no campo Utilizadores, selecione o nome de utilizador para o utilizador que pretende investigar. Pode selecionar mais do que um utilizador de cada vez.
1. Selecione Pesquisar. As atividades aparecem nos Resultados.
1. Para ver detalhes, selecione uma atividade e, em seguida, selecione Mais Informações. Na secção Parâmetros pode ver o nome da regra, as condições definidas e as ações que a regra irá tomar.

Para saber mais, consulte o registo de auditoria do Office 365 para resolver cenários comuns.