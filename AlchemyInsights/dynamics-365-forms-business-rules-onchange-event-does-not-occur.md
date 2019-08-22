---
title: Regras de negócio - regra de negócio não vai ser accionado para um formulário de formulários do Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529030"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Evento OnChange não ocorre se o campo é alterado de forma programática

O evento *OnChange* não ocorre se o campo é alterado de forma programática utilizando o *atributo.* método [DefinirValor](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Se pretender que os processadores de eventos para o evento *OnChange* ser executado depois de definir o valor tem de utilizar o *atributo formContext.data.entity.* método de [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) do código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
