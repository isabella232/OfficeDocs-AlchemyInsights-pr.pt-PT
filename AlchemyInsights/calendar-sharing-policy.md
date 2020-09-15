---
title: 618 Política de Partilha de Calendários
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684241"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="0c8d8-102">Erro de política ao partilhar um calendário</span><span class="sxs-lookup"><span data-stu-id="0c8d8-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="0c8d8-103">Faça uma das seguintes, conforme apropriado para a sua situação:</span><span class="sxs-lookup"><span data-stu-id="0c8d8-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="0c8d8-104">Conecte-se a Exchange Online utilizando o Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="0c8d8-105">Para obter mais informações, consulte [Connect to Exchange Online utilizando Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0c8d8-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="0c8d8-106">No servidor no local, abra a Shell de Gestão de Câmbios.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="0c8d8-107">Determine a política de partilha que é atribuída ao utilizador.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="0c8d8-108">Para isso, executar o seguinte comando e observar a apólice devolvida:</span><span class="sxs-lookup"><span data-stu-id="0c8d8-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="0c8d8-109">Atualize a política de partilha para o utilizador.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="0c8d8-110">Para tal, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="0c8d8-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="0c8d8-111">Abra o centro de administração Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="0c8d8-112">Clique em **Organização**e, em seguida, clique duas vezes na política que é atribuída ao utilizador em **Partilha Individual**.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="0c8d8-113">Esta é a política que foi devolvida no passo 2.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="0c8d8-114">Na página 'Regra de Partilha', selecione o nível de partilha de calendário que pretende permitir em **Especificar as informações que pretende partilhar;** clique **em Guardar**.</span><span class="sxs-lookup"><span data-stu-id="0c8d8-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="0c8d8-115">Para obter mais informações consulte: ["A política não permite a concessão de permissões a este nível a um ou mais erros do destinatário quando o utilizador tenta partilhar o calendário](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="0c8d8-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
