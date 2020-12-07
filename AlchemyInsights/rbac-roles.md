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
# <a name="rbac-rules"></a>Regras do RBAC

Se tiver o erro de permissão: 

- **O cliente com identificação de objetos não tem autorização para realizar ação sobre âmbito (código: AutorizaçãoFailed)**: quando tentar criar um recurso, verifique se está atualmente inscrito com um utilizador que é atribuído a uma função que tenha escrito permissão para o recurso no âmbito selecionado. Por exemplo, para gerir máquinas virtuais num grupo de recursos, deverá ter a função [de Contribuinte de Máquina Virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) no grupo de recursos (ou âmbito dos pais). Para obter uma lista das permissões para cada papel incorporado, consulte [as funções incorporadas para os recursos da Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Não tem permissão para criar um pedido de suporte:** quando tentar criar ou atualizar um bilhete de suporte, verifique se está atualmente inscrito com um utilizador que tem uma função que tem a permissão Microsoft.Support/supportTickets/write, como [o Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Não podem ser criadas mais atribuições de funções (código: RoleAssignmentLimitExceeded)**: quando tentar atribuir uma função, tente reduzir o número de atribuições de funções atribuindo papéis a grupos. O Azure suporta até **2000** atribuições de funções por subscrição.

Para mais detalhes sobre os papéis do Azure RBAC, consulte [os papéis do Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
