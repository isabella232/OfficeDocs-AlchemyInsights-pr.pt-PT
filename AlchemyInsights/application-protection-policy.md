---
title: Política de proteção de aplicações
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423964"
---
# <a name="application-protection-policy"></a><span data-ttu-id="cd75a-102">Política de proteção de aplicações</span><span class="sxs-lookup"><span data-stu-id="cd75a-102">Application protection policy</span></span>

<span data-ttu-id="cd75a-103">Se é novo na política de proteção de aplicações (APP), consulte a visão geral das [políticas de proteção](https://docs.microsoft.com/intune/apps/app-protection-policy)da App.</span><span class="sxs-lookup"><span data-stu-id="cd75a-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="cd75a-104">Para começar a utilizar a APP, consulte [Como criar e atribuir políticas de proteção de aplicações.](https://docs.microsoft.com/intune/app-protection-policies)</span><span class="sxs-lookup"><span data-stu-id="cd75a-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="cd75a-105">Requisitos da política de proteção de aplicações:</span><span class="sxs-lookup"><span data-stu-id="cd75a-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="cd75a-106">O utilizador tem uma licença Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="cd75a-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="cd75a-107">O utilizador pertence a um grupo visado pelas políticas de proteção de aplicações.</span><span class="sxs-lookup"><span data-stu-id="cd75a-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="cd75a-108">Apenas um utilizador corporativo é assinado em aplicações protegidas num dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd75a-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="cd75a-109">A aplicação implementou o [Intune SDK.](https://docs.microsoft.com/intune/app-sdk-get-started)</span><span class="sxs-lookup"><span data-stu-id="cd75a-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="cd75a-110">Para obter uma lista de aplicações que suportam o SDK, consulte [as aplicações protegidas do Microsoft Intune.](https://docs.microsoft.com/intune/apps-supported-intune-apps)</span><span class="sxs-lookup"><span data-stu-id="cd75a-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="cd75a-111">As políticas aplicam-se depois de um utilizador que satisfaça os sinais acima referidos numa aplicação ativada pelo Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="cd75a-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="cd75a-112">A forma mais fácil de determinar se uma apólice é aplicada é exigindo que o utilizador estabeleça um pino na apólice.</span><span class="sxs-lookup"><span data-stu-id="cd75a-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="cd75a-113">Para obter mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="cd75a-113">For more information, see:</span></span>

[<span data-ttu-id="cd75a-114">APP/MAM resolução de problemas faQ</span><span class="sxs-lookup"><span data-stu-id="cd75a-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="cd75a-115">Como validar a configuração da sua política de proteção de aplicações</span><span class="sxs-lookup"><span data-stu-id="cd75a-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="cd75a-116">Compreender o tempo de entrega da Política de Proteção de Aplicações</span><span class="sxs-lookup"><span data-stu-id="cd75a-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="cd75a-117">Como monitorizar as políticas de proteção de aplicações</span><span class="sxs-lookup"><span data-stu-id="cd75a-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)