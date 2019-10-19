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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="aacf1-102">Evento OnChange não ocorre se o campo é alterado programaticamente</span><span class="sxs-lookup"><span data-stu-id="aacf1-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="aacf1-103">O evento *onChange* não ocorre se o campo é alterado programaticamente usando o *atributo.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) método.</span><span class="sxs-lookup"><span data-stu-id="aacf1-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="aacf1-104">Se você deseja que os manipuladores de eventos para o evento *onChange* sejam executados depois de definir o valor, você deve usar o *atributo FormContext. Data. Entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) método em seu código.</span><span class="sxs-lookup"><span data-stu-id="aacf1-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
