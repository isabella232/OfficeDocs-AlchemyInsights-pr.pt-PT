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
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976876"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a atividade da regra da caixa de entrada nos registos de auditoria

Pode utilizar a pesquisa de registos de auditoria no Centro de Conformidade Microsoft 365 Segurança do & para ver os eventos de regras de caixa de entrada (criar, modificar e eliminar regras de caixa de entrada).

1. In iniciar sessão no [Centro Microsoft 365 conformidade.](https://protection.office.com/)

2. Aceda à página **Pesquisa de registo** de auditoria  >  **de** pesquisa.

3. Selecione o intervalo de **datas nos campos Data de início** e Data **de** fim.

4. Em **Exchange** Atividades da Caixa de Correio, verifique se o campo Atividades está definido para Nova Caixa de Entrada **Criar/modificar/ativar/desativar** a regra de caixa de entrada . 

5. Clique **em Procurar**.

Nos resultados, selecione um registo de auditoria. Na panfleto de detalhes, clique **em Mais Informações.** As informações sobre as definições da regra de caixa de entrada são apresentadas no **campo Parâmetros.**

Para obter mais informações, consulte [Determinar se um utilizador criou uma regra de caixa de entrada](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
