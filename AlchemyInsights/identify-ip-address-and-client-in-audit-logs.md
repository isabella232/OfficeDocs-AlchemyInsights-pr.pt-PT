---
title: Identificar endereço IP e cliente em registos de auditoria
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508927"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ed87e-102">Identificar endereço IP e cliente em registos de auditoria</span><span class="sxs-lookup"><span data-stu-id="ed87e-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ed87e-103">O endereço IP que corresponde a uma atividade de um utilizador ou administrador microsoft 365 é mostrado nos Registos de Auditoria.</span><span class="sxs-lookup"><span data-stu-id="ed87e-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ed87e-104">A informação do cliente também está registada.</span><span class="sxs-lookup"><span data-stu-id="ed87e-104">The client information is also logged.</span></span> <span data-ttu-id="ed87e-105">Aqui estão os passos para identificar tais informações</span><span class="sxs-lookup"><span data-stu-id="ed87e-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ed87e-106">Faça login no [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ed87e-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ed87e-107">Aceda à página de pesquisa de registo de registo de auditoria **de pesquisa.**  >  **Audit log search**</span><span class="sxs-lookup"><span data-stu-id="ed87e-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ed87e-108">Se estiver interessado numa atividade específica, selecione-a da lista **de Atividades.**</span><span class="sxs-lookup"><span data-stu-id="ed87e-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ed87e-109">Caso contrário, todas as atividades serão devolvidas para o utilizador selecionado (definição predefinição).</span><span class="sxs-lookup"><span data-stu-id="ed87e-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ed87e-110">**Nota:** Certas atividades podem não estar disponíveis no menu **Atividades;** no entanto, esses itens de auditoria serão devolvidos se **os Resultados do Show para todas as atividades** forem selecionados (definição predefinida).</span><span class="sxs-lookup"><span data-stu-id="ed87e-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ed87e-111">Especifique o nome de utilizador no campo **Utilizadores,** selecione o intervalo de datas apropriado para a atividade e, em seguida, clique em **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="ed87e-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ed87e-112">Nos resultados, pode ver o endereço IP para essa atividade no painel de resultados.</span><span class="sxs-lookup"><span data-stu-id="ed87e-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ed87e-113">Selecione o registo de auditoria para ver informações **detalhadas** no flyout Details (por exemplo, Cliente, Utilizador que realizou ação, etc.).</span><span class="sxs-lookup"><span data-stu-id="ed87e-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ed87e-114">Para obter mais informações, consulte [encontrar o endereço IP do computador utilizado para aceder a uma conta comprometida.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)</span><span class="sxs-lookup"><span data-stu-id="ed87e-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
