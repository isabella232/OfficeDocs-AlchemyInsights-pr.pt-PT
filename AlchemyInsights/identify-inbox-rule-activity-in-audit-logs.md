---
title: Identificar atividade de regra de caixa de entrada em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779062"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="061f5-102">Identificar atividade de regra de caixa de entrada em registos de auditoria</span><span class="sxs-lookup"><span data-stu-id="061f5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="061f5-103">Pode utilizar a pesquisa de registos de auditoria no Microsoft 365 Security & Compliance Center para visualizar eventos de regras de caixa de entrada (criando, modificando e eliminando as regras da caixa de entrada).</span><span class="sxs-lookup"><span data-stu-id="061f5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="061f5-104">Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="061f5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="061f5-105">Aceda à página de pesquisa de registo de registo de auditoria **de pesquisa.**  >  **Audit log search**</span><span class="sxs-lookup"><span data-stu-id="061f5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="061f5-106">Selecione o intervalo de datas nos campos **data de início** e **fim.**</span><span class="sxs-lookup"><span data-stu-id="061f5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="061f5-107">No âmbito **das Atividades da Caixa de Correio de Troca**, verifique se o campo de **Atividades** está definido para **a regra de Criação/Modificação/Ativação/Desativação/Desativação**.</span><span class="sxs-lookup"><span data-stu-id="061f5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="061f5-108">Clique **em Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="061f5-108">Click **Search**.</span></span>

<span data-ttu-id="061f5-109">Nos resultados, selecione um registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="061f5-109">In the results, select an audit record.</span></span> <span data-ttu-id="061f5-110">No voo de informação, clique em **Mais Informações.**</span><span class="sxs-lookup"><span data-stu-id="061f5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="061f5-111">As informações sobre as definições da regra da caixa de entrada são apresentadas no campo **Parâmetros.**</span><span class="sxs-lookup"><span data-stu-id="061f5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="061f5-112">Para obter mais informações, consulte [determine se um utilizador criou uma regra de caixa de entrada](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="061f5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
