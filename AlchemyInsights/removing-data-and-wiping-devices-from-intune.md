---
title: Desativar dados e apagar dispositivos do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416324"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="2d77b-102">Desativar dados e apagar dispositivos do Intune</span><span class="sxs-lookup"><span data-stu-id="2d77b-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="2d77b-103">As ações remotas de Desativar Dispositivo e Eliminar Todos os Dados do Dispositivo podem ser utilizadas para remover dados da empresa geridos pelo Intune ou para executar uma reposição de fábrica e restaurar o dispositivo para as suas definições padrão.</span><span class="sxs-lookup"><span data-stu-id="2d77b-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="2d77b-104">Inicie sessão na Gestão de Dispositivos do Microsoft 365, e aceda a **Dispositivos** > **Todos os Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2d77b-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="2d77b-105">Selecione o dispositivo cujos dados pretende apagar.</span><span class="sxs-lookup"><span data-stu-id="2d77b-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="2d77b-106">Selecione o tipo de eliminação remota de dados que pretende efetuar.</span><span class="sxs-lookup"><span data-stu-id="2d77b-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="2d77b-107">A desativação elimina apenas as informações da organização, ao passo que a eliminação de todos os dados repõe o dispositivo para as suas definições de fábrica.</span><span class="sxs-lookup"><span data-stu-id="2d77b-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="2d77b-108">Selecione **Sim** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="2d77b-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="2d77b-109">Até que o a eliminação de todos os dados esteja concluída, o estado de ação do Dispositivo é apresentado como *Desativação Pendente*.</span><span class="sxs-lookup"><span data-stu-id="2d77b-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="2d77b-110">Após concluir a ação, deixará de ver o dispositivo móvel na lista de dispositivos geridos.</span><span class="sxs-lookup"><span data-stu-id="2d77b-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="2d77b-111">Os dados da empresa não podem ser removidos dos dispositivos ASSOCIADOS ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2d77b-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="2d77b-112">Para obter detalhes completos sobre o efeito das ações Desativar e Eliminar todos os dados, incluindo o que é retido e eliminado, consulte a seguinte documentação:</span><span class="sxs-lookup"><span data-stu-id="2d77b-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="2d77b-113">[Remover dispositivos ao usar a eliminação de todos os dados, a desativação ou ao cancelar manualmente o registo do dispositivo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="2d77b-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="2d77b-114">Como eliminar apenas os dados empresariais de aplicações geridas pelo Intune</span><span class="sxs-lookup"><span data-stu-id="2d77b-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="2d77b-115">[Eliminar todos os dados de um dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="2d77b-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>