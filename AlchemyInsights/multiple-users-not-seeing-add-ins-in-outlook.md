---
title: Vários utilizadores que não vêem add-ins no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198238"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="b5c1e-102">Vários utilizadores que não vêem add-ins no Outlook</span><span class="sxs-lookup"><span data-stu-id="b5c1e-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="b5c1e-103">Se testar os add-ins do Outlook e nenhum aparecer, como um primeiro passo de resolução de problemas, utilize o cmdlet **Get-OrganizationConfig** PowerShell para consultar o parâmetro _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="b5c1e-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="b5c1e-104">Se a consulta devolver um valor de **Falso,** desafie este parâmetro para **True** utilizando o **cmdlet Set-OrganizationConfig,** para que os add-ins apareçam como esperado.</span><span class="sxs-lookup"><span data-stu-id="b5c1e-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="b5c1e-105">Não recomendamos que o parâmetro _AppsForOfficeEnabled_ esteja definido como **Falso**.</span><span class="sxs-lookup"><span data-stu-id="b5c1e-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="b5c1e-106">Um valor de **Falso** sobrepõe-se a todas as definições de funções administrativas e de utilizador acima e impede que quaisquer novas aplicações sejam ativadas por qualquer utilizador da organização.</span><span class="sxs-lookup"><span data-stu-id="b5c1e-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="b5c1e-107">Para obter mais informações, consulte [Especificar os administradores e utilizadores que podem instalar e gerir os add-ins para o Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="b5c1e-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>