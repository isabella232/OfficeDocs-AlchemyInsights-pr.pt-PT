---
title: Configurações de arranque no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409234"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="17bb5-102">Configurações de arranque no Windows 10</span><span class="sxs-lookup"><span data-stu-id="17bb5-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="17bb5-103">**Alterar quais as aplicações que funcionam automaticamente no arranque**</span><span class="sxs-lookup"><span data-stu-id="17bb5-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="17bb5-104">Vá a [Definições > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="17bb5-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="17bb5-105">Certifique-se de que qualquer aplicação que pretenda executar no arranque está **ligada**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="17bb5-106">**Adicione uma aplicação para executar automaticamente no arranque**</span><span class="sxs-lookup"><span data-stu-id="17bb5-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="17bb5-107">Clique ou toque **em Iniciar** e encontre a app que pretende executar no arranque.</span><span class="sxs-lookup"><span data-stu-id="17bb5-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="17bb5-108">Clique na aplicação, clique em **Mais,** e clique na localização do **ficheiro Open**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="17bb5-109">Isto abre o local onde o atalho para a aplicação é guardado.</span><span class="sxs-lookup"><span data-stu-id="17bb5-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="17bb5-110">Se não houver opção para a localização do ficheiro Open, significa que a aplicação não pode funcionar no arranque.</span><span class="sxs-lookup"><span data-stu-id="17bb5-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="17bb5-111">Com a localização do ficheiro aberta, prima a **tecla do logótipo do Windows + R,** tipo **shell:startup,** e, em seguida, clique EM **OK**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="17bb5-112">Isto abre a pasta Startup.</span><span class="sxs-lookup"><span data-stu-id="17bb5-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="17bb5-113">Copie e cole o atalho na aplicação desde a localização do ficheiro até à pasta Startup.</span><span class="sxs-lookup"><span data-stu-id="17bb5-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="17bb5-114">**Opções avançadas de arranque (incluindo Modo Seguro, definições UEFI e arranque de outro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="17bb5-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="17bb5-115">Guarde o seu trabalho e feche quaisquer documentos abertos, uma vez que estes passos irão reiniciar o seu PC.</span><span class="sxs-lookup"><span data-stu-id="17bb5-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="17bb5-116">Vá a [Definições > Atualizar & Recuperação](ms-settings:recovery?activationSource=GetHelp)de > de Segurança .</span><span class="sxs-lookup"><span data-stu-id="17bb5-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="17bb5-117">Em **arranque avançado,** clique **em Reiniciar agora**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="17bb5-118">Depois de o pc reiniciar para o ecrã Escolha um ecrã de opção:</span><span class="sxs-lookup"><span data-stu-id="17bb5-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="17bb5-119">Para arrancar de um dispositivo como uma unidade USB, clique **em Utilizar um dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="17bb5-120">Para introduzir as definições UEFI (por vezes chamada de configuração BIOS), clique em **Troubleshoot > Opções avançadas > Definições de Firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="17bb5-121">Para introduzir o Modo Seguro ou alterar as definições avançadas de arranque, clique em **Resolução de problemas > opções avançadas > Definições**de Arranque e, em seguida, clique em **Reiniciar**.</span><span class="sxs-lookup"><span data-stu-id="17bb5-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="17bb5-122">Pode ser-lhe pedido que introduza a [sua chave de recuperação BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="17bb5-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="17bb5-123">Depois de o seu PC recomeçar, clique na definição de arranque que pretende utilizar.</span><span class="sxs-lookup"><span data-stu-id="17bb5-123">After your PC restarts again, click the startup setting you want to use.</span></span>