---
title: Utilize a opção de desbloqueio de impressões digitais no Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796688"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="f6d85-102">Utilize a opção de desbloqueio de impressões digitais no Windows 10</span><span class="sxs-lookup"><span data-stu-id="f6d85-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="f6d85-103">**Ativar a impressão digital do Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="f6d85-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="f6d85-104">Para desbloquear o Windows 10 utilizando a sua impressão digital, é necessário configurar a Impressão Digital Windows Hello adicionando (permitindo que o Windows aprenda a reconhecer) pelo menos um dedo.</span><span class="sxs-lookup"><span data-stu-id="f6d85-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="f6d85-105">Aceda a **Definições > Contas > opções de inscrição** (ou clique [aqui).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="f6d85-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f6d85-106">As opções de inscrição disponíveis serão listadas.</span><span class="sxs-lookup"><span data-stu-id="f6d85-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="f6d85-107">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="f6d85-107">For example:</span></span>

    ![Opções de inscrição.](media/sign-in-options.png)

2. <span data-ttu-id="f6d85-109">Clique ou toque no **Windows Hello Fingerprint** e, em seguida, clique em **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="f6d85-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="f6d85-110">Na janela de configuração Do Windows Hello, clique **em Iniciar**.</span><span class="sxs-lookup"><span data-stu-id="f6d85-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="f6d85-111">O sensor de impressões digitais será ativado, e ser-lhe-á pedido que coloque o dedo no sensor:</span><span class="sxs-lookup"><span data-stu-id="f6d85-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor de impressões digitais.](media/fingerprint-sensor.png)

3. <span data-ttu-id="f6d85-113">Siga as instruções, que lhe pedirão para digitalizar repetidamente o dedo.</span><span class="sxs-lookup"><span data-stu-id="f6d85-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="f6d85-114">Quando isto estiver terminado, terá a opção de adicionar outros dedos que pode querer usar para iniciar sinsus.</span><span class="sxs-lookup"><span data-stu-id="f6d85-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="f6d85-115">Da próxima vez que iniciar sôs no Windows 10, terá a opção de usar a sua impressão digital para o fazer.</span><span class="sxs-lookup"><span data-stu-id="f6d85-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="f6d85-116">**Windows Hello Fingerprint não disponível como opção de inscrição**</span><span class="sxs-lookup"><span data-stu-id="f6d85-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="f6d85-117">Se o Windows Hello Fingerprint não for apresentado como uma opção nas **opções de inscrição,** significa que o Windows não tem conhecimento de nenhum leitor/scanner de impressões digitais anexado ao seu PC, ou que uma política do sistema impede a sua utilização (se, por exemplo, o seu PC for gerido pelo seu local de trabalho).</span><span class="sxs-lookup"><span data-stu-id="f6d85-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="f6d85-118">Para resolver problemas:</span><span class="sxs-lookup"><span data-stu-id="f6d85-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="f6d85-119">Selecione o botão **Iniciar** na barra de tarefas e procure **por Gestor de Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="f6d85-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="f6d85-120">Clique ou toque para abrir o **Gestor de Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="f6d85-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="f6d85-121">No Device Manager, expanda os dispositivos Biométricos clicando no seu chevron.</span><span class="sxs-lookup"><span data-stu-id="f6d85-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. <span data-ttu-id="f6d85-123">O seu scanner de impressões digitais deve ser listado como um dispositivo biométrico, como o scanner Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="f6d85-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="f6d85-125">Se o seu scanner de impressões digitais não for mostrado e o scanner estiver integrado no seu PC, aceda ao site do fabricante do PC.</span><span class="sxs-lookup"><span data-stu-id="f6d85-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="f6d85-126">Na secção de suporte técnico do seu modelo para PC, procure um controlador Windows 10 para obter um scanner que possa instalar.</span><span class="sxs-lookup"><span data-stu-id="f6d85-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="f6d85-127">Se o scanner estiver separado do PC (ligado via USB), vá ao site do fabricante do scanner para encontrar e instalar o software do controlador do dispositivo Windows 10 para o modelo de scanner que tem.</span><span class="sxs-lookup"><span data-stu-id="f6d85-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
