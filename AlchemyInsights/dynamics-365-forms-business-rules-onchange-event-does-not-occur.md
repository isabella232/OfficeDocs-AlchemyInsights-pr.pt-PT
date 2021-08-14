---
title: Regras Do Dynamics 365 Forms Business - Regra de Negócio Não Está a Funcionar para um Formulário
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947310"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>O evento AoAlterar não ocorre se o campo for alterado por programação

O *evento AoAlterar* não ocorre se o campo for alterado através de programação através do *atributo.* [método definirValor.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Se quiser que os processamentos de eventos do evento *AoAlterar* sejam executados após definir o valor, tem de utilizar o método *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) no seu código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
