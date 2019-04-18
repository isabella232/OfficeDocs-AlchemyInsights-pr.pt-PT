---
title: Identificar a actividade de regra de pasta a receber em registos de auditoria
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909462"
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
