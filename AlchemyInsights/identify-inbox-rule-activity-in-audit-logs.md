---
title: Identificar a atividade da regra da caixa de entrada nos registos de auditoria
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331134"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a atividade da regra da caixa de entrada nos registos de auditoria

Pode utilizar a pesquisa do registo de auditoria no Centro de Conformidade do Microsoft 365 para ver os eventos de regras de caixa de entrada (criar, modificar e eliminar regras de caixa de entrada).

1. Eis um dos seguintes passos:
   - Na Centro de Conformidade do Microsoft 365 em <https://compliance.microsoft.com> , vá para Auditoria de  \> **Soluções**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://compliance.microsoft.com/auditlogsearch> .
   - No portal Microsoft 365 Defender, em <https://security.microsoft.com> , vá para **Auditoria**. Em vez disso, para ir diretamente para **a página** Auditoria, utilize <https://security.microsoft.com/auditlogsearch> .

2. No **separador** Procurar da **página** Auditoria, configure as seguintes definições:
   - **Intervalo de data e hora:** selecione o intervalo de data/hora nas **caixas** Início **e** Fim.
   - **Atividades:** selecione um ou mais dos seguintes valores:
     - **Nova Regra de Caixa de Entrada Criar regra de caixa de entrada a partir Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Atualizar regras de caixa de entrada Outlook cliente**

3. Quando terminar, clique em **Procurar**. As atividades são apresentadas na nova página **Pesquisa de** auditoria.

4. Selecione uma atividade nos resultados para abrir a panfleto de detalhes. As informações sobre as definições da regra de caixa de entrada são apresentadas no **campo Parâmetros.**

Para obter mais informações, consulte [Determinar se um utilizador criou uma regra de caixa de entrada.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
