---
title: Monitorização existente da resolução de problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824590"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="bfe61-102">Resolução de problemas de um monitor existente</span><span class="sxs-lookup"><span data-stu-id="bfe61-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="bfe61-103">Experimente estas soluções para resolver problemas num monitor.</span><span class="sxs-lookup"><span data-stu-id="bfe61-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="bfe61-104">**Refresque o visor do monitor:**</span><span class="sxs-lookup"><span data-stu-id="bfe61-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="bfe61-105">Prima as seguintes teclas ao mesmo tempo: Tecla do Windows + Ctrl + Shift + B. Isto irá refrescar a comunicação com o seu controlador gráfico.</span><span class="sxs-lookup"><span data-stu-id="bfe61-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="bfe61-106">Os seus monitores piscarão momentaneamente e voltarão após alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="bfe61-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="bfe61-107">**Hardware do monitor de resolução de problemas:**</span><span class="sxs-lookup"><span data-stu-id="bfe61-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="bfe61-108">Desligue o cabo que liga o seu PC ao monitor e volte a ligá-lo.</span><span class="sxs-lookup"><span data-stu-id="bfe61-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="bfe61-109">Desligue quaisquer dispositivos não essenciais do seu PC (tais como adaptadores ou docas).</span><span class="sxs-lookup"><span data-stu-id="bfe61-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="bfe61-110">**Se instalou recentemente uma atualização no seu PC, pode reverter o controlador de exibição:**</span><span class="sxs-lookup"><span data-stu-id="bfe61-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="bfe61-111">Selecione **Iniciar,** digitar **o gestor do dispositivo** e selecione Device **Manager** a partir dos resultados.</span><span class="sxs-lookup"><span data-stu-id="bfe61-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="bfe61-112">Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito do adaptador de ecrã e selecione **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="bfe61-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="bfe61-113">Navegue no **separador Condutor** e selecione **Roll Back Driver**.</span><span class="sxs-lookup"><span data-stu-id="bfe61-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="bfe61-114">Nota: Se isto não estiver disponível ou estiver acinzentado, selecione **Não** das opções abaixo para passar para o passo seguinte.</span><span class="sxs-lookup"><span data-stu-id="bfe61-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="bfe61-115">Pode ser necessário reiniciar o seu PC antes que estas alterações entrem em vigor.</span><span class="sxs-lookup"><span data-stu-id="bfe61-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="bfe61-116">**Desinstalar e reinstalar o controlador de exibição:**</span><span class="sxs-lookup"><span data-stu-id="bfe61-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="bfe61-117">Selecione **Iniciar,** digitar **o gestor do dispositivo** e selecione Device **Manager** a partir dos resultados.</span><span class="sxs-lookup"><span data-stu-id="bfe61-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="bfe61-118">Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito do adaptador de ecrã e selecione **o dispositivo Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="bfe61-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="bfe61-119">Selecione a caixa ao lado **de Eliminar o software do controlador para este dispositivo** e selecione **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="bfe61-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="bfe61-120">Nota: Pode ser-lhe pedido que reinicie o computador nesta fase.</span><span class="sxs-lookup"><span data-stu-id="bfe61-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="bfe61-121">Certifique-se de que anota as restantes instruções antes de reiniciar.</span><span class="sxs-lookup"><span data-stu-id="bfe61-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="bfe61-122">Abra o Gestor de Dispositivos novamente.</span><span class="sxs-lookup"><span data-stu-id="bfe61-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="bfe61-123">Expanda a secção **de adaptadores do Ecrã,** clique com o botão direito no adaptador de ecrã e selecione **'Actualizar' Driver**.</span><span class="sxs-lookup"><span data-stu-id="bfe61-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="bfe61-124">Selecione **Procurar automaticamente para atualizar o software do controlador** e siga as instruções de instalação.</span><span class="sxs-lookup"><span data-stu-id="bfe61-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>