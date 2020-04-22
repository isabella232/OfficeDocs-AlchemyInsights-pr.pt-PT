---
title: Identificar a atividade da regra da caixa de entrada em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716435"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="aa214-102">Identificar a atividade da regra da caixa de entrada em registos de auditoria</span><span class="sxs-lookup"><span data-stu-id="aa214-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="aa214-103">Pode utilizar a pesquisa de registo de auditoria no Microsoft 365 Security & Compliance Center para visualizar eventos de regras de caixa de entrada (criando, modificando e eliminando as regras da caixa de entrada).</span><span class="sxs-lookup"><span data-stu-id="aa214-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="aa214-104">Inicie sessão no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="aa214-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="aa214-105">Aceda à página de pesquisa de registo de auditoria de > **pesquisa.** **Search**</span><span class="sxs-lookup"><span data-stu-id="aa214-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="aa214-106">Selecione o intervalo de data sintetiza-se nos campos de data de **início** e data de **fim.**</span><span class="sxs-lookup"><span data-stu-id="aa214-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="aa214-107">No âmbito das atividades da Caixa de Correio de **Troca,** verifique se o campo **de Atividades** está definido para **a regra de criar/modificar/ativar/desativar a caixa**de entrada .</span><span class="sxs-lookup"><span data-stu-id="aa214-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="aa214-108">Clique em **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="aa214-108">Click **Search**.</span></span>

<span data-ttu-id="aa214-109">Nos resultados, selecione um registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="aa214-109">In the results, select an audit record.</span></span> <span data-ttu-id="aa214-110">Nos detalhes, clique em **Mais Informações.**</span><span class="sxs-lookup"><span data-stu-id="aa214-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="aa214-111">As informações sobre as definições da regra da caixa de entrada são apresentadas no campo **Parâmetros.**</span><span class="sxs-lookup"><span data-stu-id="aa214-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="aa214-112">Para mais informações, consulte [Determinar se um utilizador criou uma regra](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) de caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="aa214-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
