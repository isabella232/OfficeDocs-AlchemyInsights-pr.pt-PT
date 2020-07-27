---
title: Vários utilizadores obtêm acesso negado erro ao adicionar add-ins no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424171"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="ddb4b-102">Vários utilizadores obtêm acesso negado erro ao adicionar add-ins no Outlook</span><span class="sxs-lookup"><span data-stu-id="ddb4b-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="ddb4b-103">Pode especificar quais os administradores da sua organização que têm permissões para instalar e gerir suplementos para o Outlook.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="ddb4b-104">Também pode especificar quais os utilizadores da sua organização que têm permissão para instalar e gerir suplementos para seu próprio uso.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="ddb4b-105">Para mais [informações, consulte Especificar os administradores e utilizadores que podem instalar e gerir os add-ins para o Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="ddb4b-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="ddb4b-106">Para verificar se atribuiu permissões a um utilizador com sucesso, <Role Name> substitua-a pelo nome da função a verificar e execute o seguinte comando no Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="ddb4b-107">Get-ManagementRoleAssignment - Role <Role Name> " - GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="ddb4b-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="ddb4b-108">Este exemplo mostra-lhe como verificar quem atribuiu permissões para instalar add-ins na Office Store para a organização.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="ddb4b-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="ddb4b-109">PowerShell</span></span>

<span data-ttu-id="ddb4b-110">- Papel "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="ddb4b-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="ddb4b-111">Nos resultados, Get-ManagementRoleAssignment, reveja as entradas na coluna Utilizadores Eficazes.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="ddb4b-112">Para obter informações detalhadas sobre sintaxe e [parâmetros, consulte a assinatura do Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="ddb4b-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 