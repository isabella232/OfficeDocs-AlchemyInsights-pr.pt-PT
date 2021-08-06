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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923142"
---
# <a name="rbac-rules"></a>Regras de RBAC

Se receber a mensagem de erro de permissão: 

- O cliente com ID de objeto não tem autorização para efetuar ações no âmbito **(código: AuthorizationFailed):** quando tenta criar um recurso, verifique se tem atualmente a sua assinatura com um utilizador com uma função que tem permissão de escrita para o recurso no âmbito selecionado. Por exemplo, para gerir máquinas virtuais num grupo de recursos, deve ter a função de Contribuinte de Máquina [Virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) no grupo de recursos (ou âmbito principal). Para obter uma lista das permissões para cada função incorporada, consulte Funções [incorporadas para os recursos do Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Não tem permissão para criar um pedido de **suporte:** quando tenta criar ou atualizar um pedido de suporte, verifique se tem atualmente a sua conta de utilizador com uma função com a permissão Microsoft.Support/supportTickets/write, como o Contribuinte do Pedido de Suporte [.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Já não é possível criar atribuições de funções **(código: RoleAssignmentLimitExceed)**: quando tenta atribuir uma função, tente reduzir o número de atribuições de funções ao atribuir funções a grupos. O Azure suporta até **2000 atribuições** de funções por subscrição.

Para obter mais detalhes sobre as funções RBAC do Azure, consulte Funções [RBAC do Azure.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
