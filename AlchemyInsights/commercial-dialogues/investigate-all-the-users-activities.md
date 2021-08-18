---
title: Investigar as atividades de todos os utilizadores
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332354"
---
# <a name="investigate-all-the-users-activities"></a>Investigar as atividades de todos os utilizadores

Eis como fazê-lo:

1. Eis uma das seguintes ações:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria de  \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://security.microsoft.com/auditlogsearch> .

    **Nota:** se vir um aviso a indicar que precisa de ativar a funcionalidade, continue e ativa-a agora. Se a funcionalidade não estiver ativada, os resultados da pesquisa não poderão importar dados de datas anteriores.

2. No **separador** Procurar da **página** Auditoria, configure as seguintes definições:
   - **Intervalo de data e hora:** selecione o intervalo de data/hora nas **caixas** Início **e** Fim.
   - **Atividades:** se estiver interessado numa atividade específica, selecione-a a partir da lista; caso contrário, o valor **predefinido Mostrar resultados de todas** as atividades devolve todas as atividades.
   - **Utilizadores:** aceite o valor predefinido em branco para devolver resultados de todos os utilizadores ou introduza um ou mais utilizadores.

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria. Verá o endereço **IP, Utilizador** **e** Nome **da** Atividade.

4. Para transferir os resultados, selecione **Exportar** \> **Transferir todos os Resultados**.

5. Selecione uma atividade nos resultados para abrir a panfleto de detalhes.

Para saber mais, consulte Procurar [no registo de auditoria para investigar problemas de suporte comuns.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
