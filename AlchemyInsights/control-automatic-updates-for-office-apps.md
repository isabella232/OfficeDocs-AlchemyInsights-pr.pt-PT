---
title: Controle atualizações automáticas para apps do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439921"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="94bd6-102">Controle atualizações automáticas para apps do Office</span><span class="sxs-lookup"><span data-stu-id="94bd6-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="94bd6-103">Por predefinição, as atualizações para Apps do Office são descarregadas automaticamente e aplicadas em segundo plano sem qualquer intervenção do utilizador.</span><span class="sxs-lookup"><span data-stu-id="94bd6-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="94bd6-104">No entanto, os administradores podem controlar a forma como as atualizações são aplicadas utilizando as definições de Atualização do Office.</span><span class="sxs-lookup"><span data-stu-id="94bd6-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="94bd6-105">As definições de atualização permitem aos administradores ativar ou desativar atualizações automáticas, mostrar ou ocultar o botão **Update Now** no Office, definir prazos de atualização e muito mais.</span><span class="sxs-lookup"><span data-stu-id="94bd6-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="94bd6-106">Para obter informações detalhadas, consulte:</span><span class="sxs-lookup"><span data-stu-id="94bd6-106">For detailed information, see:</span></span>

- [<span data-ttu-id="94bd6-107">Configurar definições de atualização para o Office</span><span class="sxs-lookup"><span data-stu-id="94bd6-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="94bd6-108">A atualização automática do Office não está ativada</span><span class="sxs-lookup"><span data-stu-id="94bd6-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="94bd6-109">Defina como o Office é atualizado depois de instalado</span><span class="sxs-lookup"><span data-stu-id="94bd6-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="94bd6-110">Para rever as definições de atualizações existentes aplicadas a uma máquina cliente, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="94bd6-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="94bd6-111">Abra o Editor de Registo saindo para **start**  >  **run**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="94bd6-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="94bd6-112">Mude para a seguinte localização e reveja as definições de Atualização do Office:</span><span class="sxs-lookup"><span data-stu-id="94bd6-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="94bd6-113">a.</span><span class="sxs-lookup"><span data-stu-id="94bd6-113">a.</span></span> <span data-ttu-id="94bd6-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="94bd6-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="94bd6-115">b.</span><span class="sxs-lookup"><span data-stu-id="94bd6-115">b.</span></span> <span data-ttu-id="94bd6-116">ClickToRun\Configuração</span><span class="sxs-lookup"><span data-stu-id="94bd6-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="94bd6-117">**Nota**  Se a tecla OfficeMgmtCOM estiver definida, poderá ver a mensagem "Atualizações são geridas pelo administrador **do**seu sistema" nas  >  **Account**  >  **Atualizações do Office**Account Office .</span><span class="sxs-lookup"><span data-stu-id="94bd6-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="94bd6-118">Para obter mais informações, consulte [Gerir atualizações para as aplicações da Microsoft 365 com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="94bd6-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  