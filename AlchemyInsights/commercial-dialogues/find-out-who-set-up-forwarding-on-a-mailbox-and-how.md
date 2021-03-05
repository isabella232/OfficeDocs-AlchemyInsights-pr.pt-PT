---
title: Descubra quem se instalou a encaminhar uma caixa de correio, e como
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482305"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="7505f-102">Descubra quem se instalou a encaminhar uma caixa de correio, e como</span><span class="sxs-lookup"><span data-stu-id="7505f-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="7505f-103">Se o reencaminhamento externo foi colocado numa caixa de correio, a atividade é auditada como parte do Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="7505f-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="7505f-104">Eis como encontrar a atividade no registo de auditoria:</span><span class="sxs-lookup"><span data-stu-id="7505f-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="7505f-105">Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="7505f-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="7505f-106">Selecione **pesquisa** >  **de registo de auditoria de pesquisa**.</span><span class="sxs-lookup"><span data-stu-id="7505f-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="7505f-107">Se vir um aviso de que precisa de ligar a auditoria, vá em frente e ligue-o agora.</span><span class="sxs-lookup"><span data-stu-id="7505f-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="7505f-108">Se esta funcionalidade não estiver ligada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="7505f-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="7505f-109">Certifique-se de que o campo **Atividades** está definido para **mostrar resultados para todas as atividades** (o padrão).</span><span class="sxs-lookup"><span data-stu-id="7505f-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="7505f-110">Especifique o intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="7505f-110">Specify the date range.</span></span> <span data-ttu-id="7505f-111">Não precisa de especificar um nome de utilizador.</span><span class="sxs-lookup"><span data-stu-id="7505f-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="7505f-112">Selecione **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="7505f-112">Select **Search**.</span></span> <span data-ttu-id="7505f-113">As atividades aparecem nos **Resultados.**</span><span class="sxs-lookup"><span data-stu-id="7505f-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="7505f-114">Selecione **Resultados do Filtro** e, em seguida, **introduza a caixa de correio** de set no campo do filtro **Desemundo.**</span><span class="sxs-lookup"><span data-stu-id="7505f-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="7505f-115">Isto devolve todas as atividades **da Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="7505f-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="7505f-116">Para ver os detalhes, selecione uma atividade e, em seguida, selecione **Mais Informações**.</span><span class="sxs-lookup"><span data-stu-id="7505f-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="7505f-117">Em **Parâmetros** pode ver o endereço de e-mail de encaminhamento que foi definido na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7505f-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="7505f-118">O **UserID** representa o utilizador que configura o reencaminhamento externo na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7505f-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="7505f-119">Para saber mais, consulte [o registo de auditoria do Office 365 para resolver cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="7505f-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>