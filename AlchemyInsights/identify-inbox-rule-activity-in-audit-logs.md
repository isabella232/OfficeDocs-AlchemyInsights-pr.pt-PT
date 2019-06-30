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
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383036"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar a actividade de regra de pasta a receber em registos de auditoria

Pode utilizar procura de registo de auditoria em & o Security Center de conformidade para ver eventos de regra de pasta a receber (criar, modificar e eliminar regras da pasta a receber).

1. Inicie sessão para o [Centro de conformidade do Office 365 segurança &](https://protection.office.com/)

2. Clique em **Procurar e de investigação** e seleccione a **Procura de registo de auditoria**.

3. Seleccione o intervalo de datas nos campos **data de início** e **data de fim** .

4. Em **Actividades de correio do Exchange**, verifique se o campo de **actividades** é definido como **InboxRule novo criar/modificar/activar/desactivar a regra de pasta a receber**.

5. Clique em **Procurar**.

Nos resultados, seleccione um registo de auditoria. Na lista de opções de detalhes, clique em **Mais informações**. Informações sobre as definições de regra de pasta a receber são apresentadas no campo **parâmetros** .

Para mais informações, consulte a [determinar se um utilizador que criou uma regra de pasta a receber](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
