---
title: Corrigir a política do arrendatário (sobreposição de ação)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695697"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="43835-102">Corrigir a política do arrendatário (sobreposição de ação)</span><span class="sxs-lookup"><span data-stu-id="43835-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="43835-103">Uma política anti-correio publicitário não-correio eletrónico no seu inquilino afetou esta mensagem.</span><span class="sxs-lookup"><span data-stu-id="43835-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="43835-104">Para rever a política, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="43835-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="43835-105">Vá ao [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), e depois vá para a Política de **Gestão** de Ameaças  >    >  [Antisspam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="43835-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="43835-106">Verifique se a **fonte de política** indica o seguinte:  **Add-Xheader/ModificarSubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="43835-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="43835-107">Em caso afirmativo, no separador **'Personalizado',** verifique as definições da política que afetou a mensagem.</span><span class="sxs-lookup"><span data-stu-id="43835-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="43835-108">É possível que as **definições Standard aplicadas** a todos os clientes da Exchange Online Protection afetassem a mensagem.</span><span class="sxs-lookup"><span data-stu-id="43835-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="43835-109">Para obter mais informações sobre as políticas de filtragem de spam, consulte [configurar as suas políticas de filtro de spam](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="43835-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
