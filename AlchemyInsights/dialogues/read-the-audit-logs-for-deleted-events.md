---
title: Leia os registos de auditoria para eventos apagados
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429826"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="d4277-102">Leia os registos de auditoria para eventos apagados</span><span class="sxs-lookup"><span data-stu-id="d4277-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="d4277-103">Eis como fazer isto:</span><span class="sxs-lookup"><span data-stu-id="d4277-103">Here's how to do this:</span></span>

1. <span data-ttu-id="d4277-104">Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="d4277-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="d4277-105">Selecione **pesquisa**  >  [**de registo de auditoria de pesquisa**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="d4277-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="d4277-106">Se vir um aviso de que precisa de ligar a funcionalidade, ligue-a agora.</span><span class="sxs-lookup"><span data-stu-id="d4277-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="d4277-107">Se a funcionalidade não estiver ligada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="d4277-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="d4277-108">Selecione **Atividades** e, em seguida, encontre **atividades de Caixa de Correio de Troca**.</span><span class="sxs-lookup"><span data-stu-id="d4277-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="d4277-109">Selecione as **mensagens eliminadas da pasta de itens eliminados** e mude as mensagens para opções de pasta de **itens eliminados.**</span><span class="sxs-lookup"><span data-stu-id="d4277-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="d4277-110">Quando terminar, clique fora do painel para minimizar o painel **de Atividades.**</span><span class="sxs-lookup"><span data-stu-id="d4277-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="d4277-111">Especifique o intervalo de datas e, em seguida, na caixa **Utilizadores,** selecione o nome de utilizador para o utilizador que pretende investigar.</span><span class="sxs-lookup"><span data-stu-id="d4277-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="d4277-112">Pode selecionar mais do que um utilizador de cada vez.</span><span class="sxs-lookup"><span data-stu-id="d4277-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="d4277-113">Selecione **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="d4277-113">Select **Search**.</span></span> <span data-ttu-id="d4277-114">As atividades aparecem nos **Resultados.**</span><span class="sxs-lookup"><span data-stu-id="d4277-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="d4277-115">Para ver os detalhes, selecione uma atividade e, em seguida, selecione **Mais Informações**.</span><span class="sxs-lookup"><span data-stu-id="d4277-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="d4277-116">Informações adicionais sobre o item eliminado, como a linha de assunto e a localização do item quando foi eliminado, são exibidas no campo **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="d4277-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="d4277-117">Não é possível restaurar itens eliminados utilizando a função de registo de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d4277-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="d4277-118">Para restaurar os itens eliminados, consulte [Recuperar itens eliminados ou e-mail na App Outlook Web](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="d4277-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="d4277-119">Para saber mais, consulte [o registo de auditoria do Office 365 para resolver cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="d4277-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
