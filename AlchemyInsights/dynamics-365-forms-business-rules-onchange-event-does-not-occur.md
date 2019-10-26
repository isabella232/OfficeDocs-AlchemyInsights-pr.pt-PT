---
title: Dynamics 365 forma regras de negócios - regra de negócios não disparar por um formulário
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529030"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>O evento OnChange não ocorre se o campo for alterado programaticamente

O evento *OnChange* não ocorre se o campo for alterado programaticamente usando o *atributo.* [método setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Se você quiser que os manipuladores de eventos para o evento *OnChange* sejam executados depois de definir o valor, você deve usar o *atributo formContext.data.entity.* [método fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) em seu código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
