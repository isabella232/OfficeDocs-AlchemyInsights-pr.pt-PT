---
title: Corrigir a política de ligação
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750604"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="3bfec-102">Corrigir a política de ligação</span><span class="sxs-lookup"><span data-stu-id="3bfec-102">Fix connection policy</span></span>

<span data-ttu-id="3bfec-103">O e-mail foi marcado como seguro e entregue na caixa de entrada do utilizador porque o endereço IP de envio estava marcado como seguro na política do Filtro de Ligação.</span><span class="sxs-lookup"><span data-stu-id="3bfec-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="3bfec-104">Para rever a política, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="3bfec-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="3bfec-105">Vá ao [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), e depois vá para a Política de **Gestão** de Ameaças  >    >  [Antisspam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="3bfec-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="3bfec-106">No separador **'Personalizado',** selecione a política do **filtro 'Ligação'** e, em seguida, selecione **a política de edição**.</span><span class="sxs-lookup"><span data-stu-id="3bfec-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="3bfec-107">Reveja a lista **de IP Allow.**</span><span class="sxs-lookup"><span data-stu-id="3bfec-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="3bfec-108">Veja se **a lista Safe** está ativada.</span><span class="sxs-lookup"><span data-stu-id="3bfec-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3bfec-109">A Microsoft subscreve fontes de emissores de confiança de terceiros.</span><span class="sxs-lookup"><span data-stu-id="3bfec-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="3bfec-110">Se **a lista "Safe"** estiver ativada, estes remetentes fidedignos não são erroneamente marcados como correio publicitário não-correio eletrónico.</span><span class="sxs-lookup"><span data-stu-id="3bfec-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="3bfec-111">Recomendo a seleção desta opção, pois reduzirá o número de falsos positivos (bom correio que é classificado como spam) que recebe.</span><span class="sxs-lookup"><span data-stu-id="3bfec-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
