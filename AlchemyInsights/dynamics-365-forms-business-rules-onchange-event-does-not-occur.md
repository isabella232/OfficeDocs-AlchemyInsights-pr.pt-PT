---
title: Dynamics 365 formulários regras de negócio-regra de negócio não disparar para um formulário
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529030"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Evento OnChange não ocorre se o campo é alterado programaticamente

O evento *onChange* não ocorre se o campo é alterado programaticamente usando o *atributo.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) método. Se você deseja que os manipuladores de eventos para o evento *onChange* sejam executados depois de definir o valor, você deve usar o *atributo FormContext. Data. Entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) método em seu código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
