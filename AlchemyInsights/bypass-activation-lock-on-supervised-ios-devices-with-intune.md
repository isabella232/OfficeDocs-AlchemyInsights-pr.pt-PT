---
title: Bloqueio de ativação de bypass em dispositivos iOS supervisionados com Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424216"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="7d641-102">Bloqueio de ativação de bypass em dispositivos iOS supervisionados com Intune</span><span class="sxs-lookup"><span data-stu-id="7d641-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="7d641-103">A capacidade de contornar o bloqueio de ativação nos dispositivos iOS facilita a recuperação do cenário em que um utilizador permite o bloqueio de ativação num dispositivo corporativo e, em seguida, sai da empresa.</span><span class="sxs-lookup"><span data-stu-id="7d641-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="7d641-104">Os requisitos necessários para contornar um bloqueio de ativação incluem:</span><span class="sxs-lookup"><span data-stu-id="7d641-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="7d641-105">Um dispositivo é "supervisionado".</span><span class="sxs-lookup"><span data-stu-id="7d641-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="7d641-106">O bloqueio de ativação é ativado com sucesso utilizando a política de restrição do dispositivo iOS no Intune.</span><span class="sxs-lookup"><span data-stu-id="7d641-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="7d641-107">Além disso, ao contornar um bloqueio de ativação, deve:</span><span class="sxs-lookup"><span data-stu-id="7d641-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="7d641-108">Possuir fisicamente o dispositivo a ser limpo.</span><span class="sxs-lookup"><span data-stu-id="7d641-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="7d641-109">Copie o código antes de emitir a limpeza.</span><span class="sxs-lookup"><span data-stu-id="7d641-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="7d641-110">**Nota:** O código de limpeza não é sensível a casos, pelo que os caracteres "-" não são necessários.</span><span class="sxs-lookup"><span data-stu-id="7d641-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="7d641-111">Para mais informações, consulte o Bloqueio de [Ativação do Bypass em dispositivos iOS supervisionados com o Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="7d641-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="7d641-112">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="7d641-112">**FAQ**</span></span>

<span data-ttu-id="7d641-113">P: **Emiti uma ação remota para remover os dados da empresa de um dispositivo, e agora está preso num estado pendente.**</span><span class="sxs-lookup"><span data-stu-id="7d641-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="7d641-114">R: Para uma ação remota para completar com sucesso, o dispositivo direcionado deve estar online e saudável.</span><span class="sxs-lookup"><span data-stu-id="7d641-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="7d641-115">Nas seguintes situações, a ação remota permanece em estado pendente durante 30 dias, ou até que o dispositivo reconheça o comando quando o dispositivo:</span><span class="sxs-lookup"><span data-stu-id="7d641-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="7d641-116">Não tem conectividade.</span><span class="sxs-lookup"><span data-stu-id="7d641-116">Does not have connectivity.</span></span>
- <span data-ttu-id="7d641-117">Perde o seu estatuto de gestão com a Intune.</span><span class="sxs-lookup"><span data-stu-id="7d641-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="7d641-118">Se achar que um dispositivo já não está a fazer o check-in e que não removerá os dados da empresa, selecione Delete.</span><span class="sxs-lookup"><span data-stu-id="7d641-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="7d641-119">A eliminação remove o registo do dispositivo de modo a que não apareça mais na lista de dispositivos Intune.</span><span class="sxs-lookup"><span data-stu-id="7d641-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="7d641-120">Para que o dispositivo volte a funcionar, o seu utilizador deve voltar a inscrever o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d641-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="7d641-121">P: **Porque é que certas ações remotas não estão disponíveis para eu usar?**</span><span class="sxs-lookup"><span data-stu-id="7d641-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="7d641-122">R: Nem todas as plataformas suportam todas as ações de dispositivos remotos.</span><span class="sxs-lookup"><span data-stu-id="7d641-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="7d641-123">As seguintes ações remotas são específicas da plataforma.</span><span class="sxs-lookup"><span data-stu-id="7d641-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="7d641-124">Bloqueio de ativação do bypass (apenas iOS)</span><span class="sxs-lookup"><span data-stu-id="7d641-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="7d641-125">Início Fresco (apenas janelas)</span><span class="sxs-lookup"><span data-stu-id="7d641-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="7d641-126">Modo perdido (apenas iOS)</span><span class="sxs-lookup"><span data-stu-id="7d641-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="7d641-127">Localizar dispositivo (apenas iOS)</span><span class="sxs-lookup"><span data-stu-id="7d641-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="7d641-128">Reiniciar (apenas para windows)</span><span class="sxs-lookup"><span data-stu-id="7d641-128">Restart (Windows only)</span></span>

<span data-ttu-id="7d641-129">Para obter mais detalhes sobre cada ação, consulte [as ações do dispositivo disponíveis.](https://docs.microsoft.com/intune/device-management#available-device-actions)</span><span class="sxs-lookup"><span data-stu-id="7d641-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>