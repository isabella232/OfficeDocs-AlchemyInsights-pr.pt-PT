---
title: 'Funções RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583949"
---
# <a name="rbac-rules"></a><span data-ttu-id="6f047-102">Regras do RBAC</span><span class="sxs-lookup"><span data-stu-id="6f047-102">RBAC rules</span></span>

<span data-ttu-id="6f047-103">Se tiver o erro de permissão:</span><span class="sxs-lookup"><span data-stu-id="6f047-103">If you get the permission error:</span></span> 

- <span data-ttu-id="6f047-104">**O cliente com identificação de objetos não tem autorização para realizar ação sobre âmbito (código: AutorizaçãoFailed)**: quando tentar criar um recurso, verifique se está atualmente inscrito com um utilizador que é atribuído a uma função que tenha escrito permissão para o recurso no âmbito selecionado.</span><span class="sxs-lookup"><span data-stu-id="6f047-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="6f047-105">Por exemplo, para gerir máquinas virtuais num grupo de recursos, deverá ter a função [de Contribuinte de Máquina Virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) no grupo de recursos (ou âmbito dos pais).</span><span class="sxs-lookup"><span data-stu-id="6f047-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="6f047-106">Para obter uma lista das permissões para cada papel incorporado, consulte [as funções incorporadas para os recursos da Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="6f047-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="6f047-107">**Não tem permissão para criar um pedido de suporte:** quando tentar criar ou atualizar um bilhete de suporte, verifique se está atualmente inscrito com um utilizador que tem uma função que tem a permissão Microsoft.Support/supportTickets/write, como [o Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="6f047-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="6f047-108">**Não podem ser criadas mais atribuições de funções (código: RoleAssignmentLimitExceeded)**: quando tentar atribuir uma função, tente reduzir o número de atribuições de funções atribuindo papéis a grupos.</span><span class="sxs-lookup"><span data-stu-id="6f047-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="6f047-109">O Azure suporta até **2000** atribuições de funções por subscrição.</span><span class="sxs-lookup"><span data-stu-id="6f047-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="6f047-110">Para mais detalhes sobre os papéis do Azure RBAC, consulte [os papéis do Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="6f047-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
