---
title: Encontrar eventos efetuado em regras de caixa de entrada
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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058661"
---
# <a name="find-events-performed-on-inbox-rules"></a>Encontrar eventos efetuado em regras de caixa de entrada

Quando as regras de caixa de entrada são criadas, alteradas ou eliminadas, os eventos são registados no registo de auditoria. Eis como revê-los:

1. Vá para o Centro [de conformidade Office 365 de & de Conformidade.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selecione Procurar > de Registo de auditoria.

    > [!NOTE]
    > Se vir um aviso a dizer que precisa de a ligar a auditoria, continue e a ligue-o agora. Se esta funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.
1. Selecione o campo Atividades e procure Exchange de caixa de correio e, em seguida, selecione New-InboxRule Criar regra de caixa de entrada a partir Outlook Web App. Quando terminar, clique fora do painel para minimizar o painel Atividades.
1. Especifique o intervalo de datas e, em seguida, no campo Utilizadores, selecione o nome de utilizador do utilizador que pretende investigar. Pode selecionar mais do que um utilizador de cada vez.
1. Selecione Procurar. As atividades são apresentadas em Resultados.
1. Para ver detalhes, selecione uma atividade e, em seguida, selecione Mais Informações. Na secção Parâmetros, pode ver o nome da regra, o conjunto de condições e as ações que a regra irá tomar.

Para saber mais, consulte Procurar no registo Office 365 de auditoria para remoção de cenários comuns.