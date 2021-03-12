---
title: Dispositivos não-Windows offboard do Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748479"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="cd7ec-102">Dispositivos não-Windows offboard do Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="cd7ec-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="cd7ec-103">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="cd7ec-103">Here's how:</span></span>

1. <span data-ttu-id="cd7ec-104">Siga a documentação de terceiros para desligar a solução de terceiros do Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="cd7ec-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="cd7ec-105">Do seu inquilino Azure Ative Directory, remova permissões para a solução de terceiros:</span><span class="sxs-lookup"><span data-stu-id="cd7ec-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="cd7ec-106">Inscreva-se no [portal Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="cd7ec-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="cd7ec-107">Selecione **Todos os serviços**  >  **Azure Ative Directory**  >  **Enterprise Applications**.</span><span class="sxs-lookup"><span data-stu-id="cd7ec-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="cd7ec-108">Selecione a aplicação que gostaria de embarcar.</span><span class="sxs-lookup"><span data-stu-id="cd7ec-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="cd7ec-109">Selecione **Eliminar**.</span><span class="sxs-lookup"><span data-stu-id="cd7ec-109">Select **Delete**.</span></span>

<span data-ttu-id="cd7ec-110">Para saber mais, consulte [dispositivos não-Windows offboard](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="cd7ec-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
