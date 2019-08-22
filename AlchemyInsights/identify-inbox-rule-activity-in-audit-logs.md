---
title: Identificar a actividade de regra de pasta a receber em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539184"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a actividade de regra de pasta a receber em registos de auditoria

Pode utilizar procura de registo de auditoria no & a segurança do Office 365 conformidade Center para ver eventos de regra de pasta a receber (criar, modificar e eliminar regras da pasta a receber).

1. Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/).

2. Vá para a **pesquisa**de > página de**procura de registo de auditoria** .

3. Seleccione o intervalo de datas nos campos **data de início** e **data de fim** .

4. Em **Actividades de correio do Exchange**, verifique se o campo de **actividades** é definido como **InboxRule novo criar/modificar/activar/desactivar a regra de pasta a receber**.

5. Clique em **Procurar**.

Nos resultados, seleccione um registo de auditoria. Na lista de opções de detalhes, clique em **Mais informações**. Informações sobre as definições de regra de pasta a receber são apresentadas no campo **parâmetros** .

Para mais informações, consulte a [determinar se um utilizador que criou uma regra de pasta a receber](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
