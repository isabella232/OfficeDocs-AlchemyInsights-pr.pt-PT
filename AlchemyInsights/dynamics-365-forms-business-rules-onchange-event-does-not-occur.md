---
title: Dinâmica 365 Formas Regras empresariais - Regra de Negócios Não Disparando para um Formulário
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711502"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>O evento OnChange não ocorre se o campo for alterado programáticamente

O evento *OnChange* não ocorre se o campo for alterado programáticamente usando o *atributo.* [definir Método de Valor.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Se quiser que os manipuladores de eventos para o evento *OnChange* seja executado depois de definir o valor, deve utilizar o *formulárioContext.data.entity atribuir* o método [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) no seu código.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
