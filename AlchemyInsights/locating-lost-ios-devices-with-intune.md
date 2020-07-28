---
title: Localizar dispositivos iOS perdidos com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440425"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="91cf7-102">Localizar dispositivos iOS perdidos com o Intune</span><span class="sxs-lookup"><span data-stu-id="91cf7-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="91cf7-103">Ativar o modo perdido num dispositivo iOS permite que um administrador tenha uma mensagem e um número de telefone de contacto apresentados no ecrã de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="91cf7-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="91cf7-104">Depois de o modo perdido ser ativado, o administrador pode utilizar a ação do dispositivo Localizar para identificar a localização física do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91cf7-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="91cf7-105">A ação do dispositivo Localizar no Intune funciona com dispositivos iOS para mostrar a localização de um dispositivo específico num mapa.</span><span class="sxs-lookup"><span data-stu-id="91cf7-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="91cf7-106">A utilização desta ação requer que o dispositivo iOS esteja em:</span><span class="sxs-lookup"><span data-stu-id="91cf7-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="91cf7-107">Modo supervisionado</span><span class="sxs-lookup"><span data-stu-id="91cf7-107">Supervised mode</span></span>
- <span data-ttu-id="91cf7-108">Modo perdido</span><span class="sxs-lookup"><span data-stu-id="91cf7-108">Lost mode</span></span>

<span data-ttu-id="91cf7-109">Para obter mais informações, consulte [Ativar o modo perdido em dispositivos iOS/iPadOS com dispositivos Intune](https://docs.microsoft.com/intune/device-lost-mode) e [Localizar dispositivos iOS/iPadOS perdidos ou roubados com Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="91cf7-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="91cf7-110">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="91cf7-110">**FAQ**</span></span>

<span data-ttu-id="91cf7-111">P: Emiti uma ação remota para remover os dados da empresa de um dispositivo, e agora está preso num estado pendente.</span><span class="sxs-lookup"><span data-stu-id="91cf7-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="91cf7-112">R: Para uma ação remota para completar com sucesso, o dispositivo direcionado deve estar online e saudável.</span><span class="sxs-lookup"><span data-stu-id="91cf7-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="91cf7-113">Nas seguintes situações, a ação remota permanece em estado pendente durante 30 dias, ou até que o dispositivo reconheça o comando:</span><span class="sxs-lookup"><span data-stu-id="91cf7-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="91cf7-114">Quando o dispositivo não tem conectividade</span><span class="sxs-lookup"><span data-stu-id="91cf7-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="91cf7-115">Quando o dispositivo perde o seu estatuto de gestão com a Intune</span><span class="sxs-lookup"><span data-stu-id="91cf7-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="91cf7-116">Se achar que um dispositivo já não está a fazer o check-in e que não será capaz de remover os dados da empresa, selecione Delete.</span><span class="sxs-lookup"><span data-stu-id="91cf7-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="91cf7-117">A eliminação remove o registo do dispositivo de modo a que não apareça mais na lista de dispositivos Intune.</span><span class="sxs-lookup"><span data-stu-id="91cf7-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="91cf7-118">Se o dispositivo voltar a funcionar, o utilizador terá de o reinscrevê-lo.</span><span class="sxs-lookup"><span data-stu-id="91cf7-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="91cf7-119">P: Porque é que certas ações remotas não estão disponíveis para eu usar?</span><span class="sxs-lookup"><span data-stu-id="91cf7-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="91cf7-120">R: Nem todas as plataformas suportam todas as ações de dispositivos remotos.</span><span class="sxs-lookup"><span data-stu-id="91cf7-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="91cf7-121">As seguintes ações remotas são específicas da plataforma, pelo que estão disponíveis apenas para as plataformas notadas.</span><span class="sxs-lookup"><span data-stu-id="91cf7-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="91cf7-122">Bloqueio de ativação do bypass (apenas iOS)</span><span class="sxs-lookup"><span data-stu-id="91cf7-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="91cf7-123">Início Fresco (apenas janelas)</span><span class="sxs-lookup"><span data-stu-id="91cf7-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="91cf7-124">Modo perdido (apenas iOS)</span><span class="sxs-lookup"><span data-stu-id="91cf7-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="91cf7-125">Localizar dispositivo (apenas iOS)</span><span class="sxs-lookup"><span data-stu-id="91cf7-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="91cf7-126">Reiniciar (apenas para windows)</span><span class="sxs-lookup"><span data-stu-id="91cf7-126">Restart (Windows only)</span></span>

<span data-ttu-id="91cf7-127">Para obter mais detalhes sobre cada ação, consulte [as ações do dispositivo disponíveis.](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="91cf7-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>