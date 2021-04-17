---
title: Definições de arranque no Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828163"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="c16d7-102">Definições de arranque no Windows 10</span><span class="sxs-lookup"><span data-stu-id="c16d7-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="c16d7-103">**Alterar quais aplicações são executadas automaticamente no arranque**</span><span class="sxs-lookup"><span data-stu-id="c16d7-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="c16d7-104">Vá a [Definições > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="c16d7-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="c16d7-105">Certifique-se de que qualquer aplicação que pretenda executar no arranque está **ligada**.</span><span class="sxs-lookup"><span data-stu-id="c16d7-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="c16d7-106">**Adicione uma app para executar automaticamente no arranque**</span><span class="sxs-lookup"><span data-stu-id="c16d7-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="c16d7-107">Clique ou toque **em Iniciar** e encontre a aplicação que pretende executar no arranque.</span><span class="sxs-lookup"><span data-stu-id="c16d7-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="c16d7-108">Clique com o botão direito na aplicação, clique em **Mais** e, em seguida, clique em **Abrir a localização do ficheiro**.</span><span class="sxs-lookup"><span data-stu-id="c16d7-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="c16d7-109">Isto abre o local onde o atalho para a aplicação é guardado.</span><span class="sxs-lookup"><span data-stu-id="c16d7-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="c16d7-110">Se não houver opção para a localização do ficheiro Aberto, significa que a aplicação não pode ser executada no arranque.</span><span class="sxs-lookup"><span data-stu-id="c16d7-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="c16d7-111">Com a localização do ficheiro aberta, prima a **tecla** do logótipo do Windows + R , tipo **shell:startup,** em seguida, clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="c16d7-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="c16d7-112">Isto abre a pasta Startup.</span><span class="sxs-lookup"><span data-stu-id="c16d7-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="c16d7-113">Copie e cole o atalho para a aplicação desde a localização do ficheiro até à pasta Startup.</span><span class="sxs-lookup"><span data-stu-id="c16d7-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="c16d7-114">**Opções avançadas de arranque (incluindo modo de segurança, definições UEFI e arranque de outro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="c16d7-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="c16d7-115">Guarde o seu trabalho e feche quaisquer documentos abertos, uma vez que estes passos reiniciarão o seu PC.</span><span class="sxs-lookup"><span data-stu-id="c16d7-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="c16d7-116">Ir para [Definições > Atualizar & recuperação > de segurança](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="c16d7-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="c16d7-117">No **arranque avançado,** clique **em Reiniciar agora**.</span><span class="sxs-lookup"><span data-stu-id="c16d7-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="c16d7-118">Depois do seu PC reiniciar para o ecrã de opção Escolha:</span><span class="sxs-lookup"><span data-stu-id="c16d7-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="c16d7-119">Para arrancar a partir de um dispositivo como uma unidade USB, clique em **Utilizar um dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="c16d7-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="c16d7-120">Para introduzir as definições UEFI (por vezes chamada configuração BIOS), clique em **Resolução de Problemas > Opções Avançadas > Definições de Firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="c16d7-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="c16d7-121">Para introduzir o Modo de Segurança ou alterar as definições avançadas de arranque, clique em **Troubleshoot > Opções Avançadas > Configurações de Arranque**, clique em **"Reiniciar"**</span><span class="sxs-lookup"><span data-stu-id="c16d7-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="c16d7-122">Pode ser-lhe pedido que introduza a sua [chave de recuperação BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="c16d7-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="c16d7-123">Depois de o seu PC recomeçar, clique na definição de arranque que pretende utilizar.</span><span class="sxs-lookup"><span data-stu-id="c16d7-123">After your PC restarts again, click the startup setting you want to use.</span></span>