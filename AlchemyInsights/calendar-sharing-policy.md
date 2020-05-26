---
title: 618 Política de Partilha de Calendários
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373010"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="145a3-102">Erro de política ao partilhar um calendário</span><span class="sxs-lookup"><span data-stu-id="145a3-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="145a3-103">Faça um dos seguintes, conforme apropriado para a sua situação:</span><span class="sxs-lookup"><span data-stu-id="145a3-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="145a3-104">Ligue-se ao Exchange Online utilizando a Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="145a3-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="145a3-105">Para mais informações, consulte [Connect to Exchange Online utilizando a Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="145a3-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="145a3-106">No servidor no local, abra a Shell exchange Management.</span><span class="sxs-lookup"><span data-stu-id="145a3-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="145a3-107">Determine a política de partilha que é atribuída ao utilizador.</span><span class="sxs-lookup"><span data-stu-id="145a3-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="145a3-108">Para tal, execute o seguinte comando e note a política devolvida:</span><span class="sxs-lookup"><span data-stu-id="145a3-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="145a3-109">Atualize a política de partilha para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="145a3-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="145a3-110">To do this, follow these steps:</span><span class="sxs-lookup"><span data-stu-id="145a3-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="145a3-111">Abra o centro de administração exchange.</span><span class="sxs-lookup"><span data-stu-id="145a3-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="145a3-112">Clique em **Organização**, e, em seguida, clique duas vezes na política atribuída ao utilizador em **Partilha Individual**.</span><span class="sxs-lookup"><span data-stu-id="145a3-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="145a3-113">Esta é a política que foi devolvida no passo 2.</span><span class="sxs-lookup"><span data-stu-id="145a3-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="145a3-114">Na página 'Regra de Partilha', selecione o nível de partilha de calendário que pretende permitir sob **especificar quais as informações que pretende partilhar;** clique **em Guardar**.</span><span class="sxs-lookup"><span data-stu-id="145a3-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="145a3-115">Para obter mais informações consulte: ["A política não permite conceder permissões a este nível a um ou mais dos(s)" erro](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)do destinatário quando o utilizador tenta partilhar o calendário .</span><span class="sxs-lookup"><span data-stu-id="145a3-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
