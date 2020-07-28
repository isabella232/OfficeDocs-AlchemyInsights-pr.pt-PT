---
title: Remoção de dados e dispositivos de limpeza do Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440470"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="23c33-102">Remoção de dados e dispositivos de limpeza do Intune</span><span class="sxs-lookup"><span data-stu-id="23c33-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="23c33-103">As ações remotas de remoção de dispositivos e limpeza de dispositivos podem ser utilizadas para remover os dados da empresa geridos pelo Intune ou para executar um reset de fábrica e devolver o dispositivo às suas definições predefinidas.</span><span class="sxs-lookup"><span data-stu-id="23c33-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="23c33-104">Inscreva-se na Microsoft 365 Device Management e vá para **dispositivos**  >  **todos os dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="23c33-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="23c33-105">Selecione o dispositivo que pretende limpar.</span><span class="sxs-lookup"><span data-stu-id="23c33-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="23c33-106">Selecione o tipo de limpeza remota que pretende fazer.</span><span class="sxs-lookup"><span data-stu-id="23c33-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="23c33-107">A aposentadoria elimina apenas informações organizacionais, enquanto as toalhetes completas devolvem o dispositivo às suas definições de fábrica.</span><span class="sxs-lookup"><span data-stu-id="23c33-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="23c33-108">Selecione **Sim** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="23c33-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="23c33-109">Até que a limpeza termine, o estado de ação do dispositivo mostra como Aposentadoria Pendente.</span><span class="sxs-lookup"><span data-stu-id="23c33-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="23c33-110">Depois de concluída a ação, deixará de ver o dispositivo móvel na lista de dispositivos geridos.</span><span class="sxs-lookup"><span data-stu-id="23c33-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="23c33-111">**Nota** Os dados da empresa não podem ser removidos dos dispositivos associados à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23c33-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="23c33-112">Para obter todos os detalhes sobre o efeito das ações retire e limpadoras, incluindo o que é retido e o que é eliminado, consulte [remover os dispositivos utilizando limpeza, aposentação ou desinsusamento manual do dispositivo](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="23c33-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="23c33-113">Para apagar todos os dados de um dispositivo macOS, consulte [apagar todos os dados de um dispositivo macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="23c33-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>