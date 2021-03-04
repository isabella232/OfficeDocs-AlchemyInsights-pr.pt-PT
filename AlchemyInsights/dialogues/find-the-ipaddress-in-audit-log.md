---
title: Encontre o endereço IP no registo de auditoria
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429787"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="d5576-102">Encontre o endereço IP no registo de auditoria</span><span class="sxs-lookup"><span data-stu-id="d5576-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="d5576-103">O endereço IP que corresponde a uma atividade realizada por um utilizador ou administrador é mostrado nos registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="d5576-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="d5576-104">A informação do cliente também está registada.</span><span class="sxs-lookup"><span data-stu-id="d5576-104">The client information is also logged.</span></span> <span data-ttu-id="d5576-105">Aqui está como identificar o endereço IP:</span><span class="sxs-lookup"><span data-stu-id="d5576-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="d5576-106">Vá ao [Centro de Segurança & Compliance do Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="d5576-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="d5576-107">Selecione **pesquisa**  >  **[de registo de auditoria de pesquisa](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="d5576-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="d5576-108">Se vir um aviso de que precisa de ligar a auditoria, vá em frente e ligue-o agora.</span><span class="sxs-lookup"><span data-stu-id="d5576-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="d5576-109">Se esta funcionalidade não estiver ativada, os resultados da pesquisa não serão capazes de extrair dados de datas anteriores.</span><span class="sxs-lookup"><span data-stu-id="d5576-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="d5576-110">Se estiver interessado numa atividade específica, selecione-a na lista **de Atividades;** caso contrário, por padrão, todas as atividades serão devolvidas para o utilizador selecionado.</span><span class="sxs-lookup"><span data-stu-id="d5576-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="d5576-111">Note que certas atividades podem não estar disponíveis para seleção a partir do menu **Atividades;** no entanto, esses itens de auditoria serão devolvidos se **os resultados do Show para todas as atividades** forem selecionados (definição predefinida).</span><span class="sxs-lookup"><span data-stu-id="d5576-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="d5576-112">Especifique o intervalo de datas e, no campo **Utilizadores,** selecione o nome de utilizador para o utilizador que pretende investigar.</span><span class="sxs-lookup"><span data-stu-id="d5576-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="d5576-113">Selecione **Pesquisar**.</span><span class="sxs-lookup"><span data-stu-id="d5576-113">Select **Search**.</span></span> <span data-ttu-id="d5576-114">As atividades aparecem nos **Resultados.**</span><span class="sxs-lookup"><span data-stu-id="d5576-114">The activities appear under **Results**.</span></span> <span data-ttu-id="d5576-115">Pode ver o endereço IP de cada atividade.</span><span class="sxs-lookup"><span data-stu-id="d5576-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="d5576-116">Para ver detalhes, selecione uma atividade e, em seguida, selecione **Mais Informações**.</span><span class="sxs-lookup"><span data-stu-id="d5576-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="d5576-117">Para saber mais, consulte o [registo de auditoria do Office 365 para resolver cenários comuns.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="d5576-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>