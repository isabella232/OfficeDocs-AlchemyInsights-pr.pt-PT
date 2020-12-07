---
title: O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583786"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="d170d-102">O que fazer se as funcionalidades do Azure não funcionarem corretamente no Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d170d-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="d170d-103">O Microsoft Edge [tem conhecido problemas relacionados](https://go.microsoft.com/fwlink/?linkid=2140608) com zonas de segurança e pode afetar a forma como os utilizadores do Azure entram no Windows Admin Center.</span><span class="sxs-lookup"><span data-stu-id="d170d-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="d170d-104">Se tiver problemas em utilizar funcionalidades do Azure com o Microsoft Edge, experimente os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="d170d-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="d170d-105">No menu **Iniciar,** procure **opções de Internet** e selecione-as.</span><span class="sxs-lookup"><span data-stu-id="d170d-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="d170d-106">Na caixa de diálogo **Internet Properties,** aceda ao **separador Segurança.**</span><span class="sxs-lookup"><span data-stu-id="d170d-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="d170d-107">Selecione a zona **de sites Fidedignos** e, em seguida, selecione o botão **'Sites'.**</span><span class="sxs-lookup"><span data-stu-id="d170d-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="d170d-108">Na caixa de diálogo **dos sites Fidedignos,** adicione o URL do gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e , [https://login.live.com](https://login.live.com) e, em seguida, selecione **Close**.</span><span class="sxs-lookup"><span data-stu-id="d170d-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="d170d-109">Na caixa de diálogo **Internet Properties,** aceda ao **separador Privacidade.**</span><span class="sxs-lookup"><span data-stu-id="d170d-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="d170d-110">Na secção **'Bloqueador Pop-up',** selecione **Definições**.</span><span class="sxs-lookup"><span data-stu-id="d170d-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="d170d-111">Na caixa de diálogo que se abre, adicione o URL do gateway bem como [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) e , e, em seguida, selecione **Close**.</span><span class="sxs-lookup"><span data-stu-id="d170d-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
