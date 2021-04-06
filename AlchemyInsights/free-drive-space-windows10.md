---
title: Libertar espaço em disco no Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505367"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="83c85-102">Libertar espaço em disco no Windows 10</span><span class="sxs-lookup"><span data-stu-id="83c85-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="83c85-103">Eis duas opções para libertar espaço em disco no Windows:</span><span class="sxs-lookup"><span data-stu-id="83c85-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="83c85-104">Liberte espaço em disco no Windows 10.</span><span class="sxs-lookup"><span data-stu-id="83c85-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="83c85-105">Liberte espaço para as atualizações do Windows 10 com dispositivos de armazenamento externo.</span><span class="sxs-lookup"><span data-stu-id="83c85-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="83c85-106">Se ainda tiver pouco espaço em disco após utilizar a Limpeza do Disco, é possível que a sua pasta Temporária esteja a ficar rapidamente cheia de ficheiros de aplicação (.appx) utilizados pela Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="83c85-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="83c85-107">Para corrigir este problema, reponha a Store, limpe a cache da Store e, em seguida, execute a resolução de problemas do Windows Update.</span><span class="sxs-lookup"><span data-stu-id="83c85-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="83c85-108">Certifique-se de que a Microsoft Store está fechada antes de seguir estes passos.</span><span class="sxs-lookup"><span data-stu-id="83c85-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="83c85-109">**Passo 1: repor a Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="83c85-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="83c85-110">**Nota** Esta ação elimina permanentemente os dados da aplicação no dispositivo, incluindo as suas preferências e detalhes de início de sessão.</span><span class="sxs-lookup"><span data-stu-id="83c85-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="83c85-111">Selecione **Iniciar** > **Definições** > **Aplicações** > **Aplicações e funcionalidades**.</span><span class="sxs-lookup"><span data-stu-id="83c85-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="83c85-112">Na lista de aplicações, localize e selecione Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="83c85-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="83c85-113">Selecione **Opções avançadas**.</span><span class="sxs-lookup"><span data-stu-id="83c85-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="83c85-114">Desloque-se para baixo e selecione **Repor** e, em seguida, **Confirmar Reposição**.</span><span class="sxs-lookup"><span data-stu-id="83c85-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="83c85-115">**Passo 2: limpar a cache da Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="83c85-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="83c85-116">Prima a tecla do logótipo do Windows + R para abrir a caixa de diálogo Executar.</span><span class="sxs-lookup"><span data-stu-id="83c85-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="83c85-117">Escreva wsreset.exe e selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="83c85-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="83c85-118">É aberta uma janela de Linha de Comandos em branco.</span><span class="sxs-lookup"><span data-stu-id="83c85-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="83c85-119">Após cerca de 10 segundos, a janela é fechada e a Store é aberta automaticamente.</span><span class="sxs-lookup"><span data-stu-id="83c85-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="83c85-120">**Passo 3: repor o Windows Update**</span><span class="sxs-lookup"><span data-stu-id="83c85-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="83c85-121">Selecione **Iniciar** > **Definições** > **Atualizar e Segurança** > **Resolução de Problemas**.</span><span class="sxs-lookup"><span data-stu-id="83c85-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="83c85-122">Desloque-se para baixo e selecione **Windows Update** a partir da lista e, em seguida, **Executar a resolução de problemas**.</span><span class="sxs-lookup"><span data-stu-id="83c85-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="83c85-123">Reinicie o computador e verifique se o problema ainda está presente.</span><span class="sxs-lookup"><span data-stu-id="83c85-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

