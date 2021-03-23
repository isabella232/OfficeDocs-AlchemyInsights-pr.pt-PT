---
title: Espaço de unidade gratuito no Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037945"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="8512e-102">Espaço de unidade gratuito no Windows 10</span><span class="sxs-lookup"><span data-stu-id="8512e-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="8512e-103">Aqui estão duas opções para libertar o espaço de condução no Windows:</span><span class="sxs-lookup"><span data-stu-id="8512e-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="8512e-104">Liberte espaço de unidade no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8512e-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="8512e-105">Liberte espaço para atualizações do Windows 10 com dispositivo de armazenamento externo.</span><span class="sxs-lookup"><span data-stu-id="8512e-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="8512e-106">Se ainda tiver pouco espaço em disco depois de utilizar a Disk Cleanup, é possível que a sua pasta Temp esteja rapidamente a preencher com ficheiros de aplicação (.appx) utilizados pela Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="8512e-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="8512e-107">Para corrigir este problema, reinicie a Loja, limpe a cache da Loja e, em seguida, execute o resolução de problemas do Windows Update.</span><span class="sxs-lookup"><span data-stu-id="8512e-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="8512e-108">Certifique-se de que a Microsoft Store está fechada antes de prosseguir com estes passos.</span><span class="sxs-lookup"><span data-stu-id="8512e-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="8512e-109">**Passo 1: Redefinir a Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="8512e-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="8512e-110">**Nota** Isto elimina permanentemente os dados da aplicação no dispositivo, incluindo as suas preferências e detalhes de início de saúde.</span><span class="sxs-lookup"><span data-stu-id="8512e-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="8512e-111">Selecione   >  **Iniciar Definições**  >    >  **Aplicações Apps & funcionalidades**.</span><span class="sxs-lookup"><span data-stu-id="8512e-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="8512e-112">Na lista de aplicações, localize e selecione a Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="8512e-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="8512e-113">Selecione **opções avançadas**.</span><span class="sxs-lookup"><span data-stu-id="8512e-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="8512e-114">Desloque-se para baixo e **selecione Reset** e, em seguida, **confirme reset**.</span><span class="sxs-lookup"><span data-stu-id="8512e-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="8512e-115">**Passo 2: Limpar a cache da Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="8512e-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="8512e-116">Prima a tecla do logotipo do Windows + R para abrir a caixa de diálogo executar.</span><span class="sxs-lookup"><span data-stu-id="8512e-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="8512e-117">Digite wsreset.exe e selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="8512e-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="8512e-118">Abre-se uma janela de pedido de comando em branco.</span><span class="sxs-lookup"><span data-stu-id="8512e-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="8512e-119">Após cerca de 10 segundos, a janela fecha-se e a Loja abre-se automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8512e-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="8512e-120">**Passo 3: Redefinir atualização do Windows**</span><span class="sxs-lookup"><span data-stu-id="8512e-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="8512e-121">Selecione **Iniciar**  >    >  **Atualização de Definições &**  >  **resolução de problemas de** segurança .</span><span class="sxs-lookup"><span data-stu-id="8512e-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="8512e-122">Desloque-se para baixo e selecione o **Windows Update** da lista e selecione **Executar o resolução de problemas**.</span><span class="sxs-lookup"><span data-stu-id="8512e-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="8512e-123">Reinicie o seu computador e verifique se ainda está a passar pelo problema.</span><span class="sxs-lookup"><span data-stu-id="8512e-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

