---
title: Problemas de áudio no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265027"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="14131-102">Problemas de resolução de problemas de áudio no Windows 10</span><span class="sxs-lookup"><span data-stu-id="14131-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="14131-103">**Executar o problema de áudio**</span><span class="sxs-lookup"><span data-stu-id="14131-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="14131-104">Abra as definições de [Troubleshoot](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="14131-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="14131-105">Selecione **Reproduzir áudio** > **Executar o resolução de problemas**.</span><span class="sxs-lookup"><span data-stu-id="14131-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="14131-106">**Definir o dispositivo predefinido**</span><span class="sxs-lookup"><span data-stu-id="14131-106">**Set the default device**</span></span>

<span data-ttu-id="14131-107">Se estiver a ligar-se a um dispositivo de áudio utilizando USB ou HDMI, poderá ter de definir esse dispositivo como predefinido:</span><span class="sxs-lookup"><span data-stu-id="14131-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="14131-108"> > Abra\ \*\*\** o**Start Sound**e, em seguida, selecione **sons** do sistema **Sound** or Change da lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="14131-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="14131-109">No **separador Reprodução,** selecione um dispositivo, selecione **'Definir Padrão**' e, em seguida, selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="14131-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="14131-110">**Verifique os cabos, volume, altifalantes e auscultadores**</span><span class="sxs-lookup"><span data-stu-id="14131-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="14131-111">Verifique se os altifalantes e os auscultadores estão ligados à tomada correta.</span><span class="sxs-lookup"><span data-stu-id="14131-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="14131-112">Verifique os níveis de potência e volume e tente aumentar todos os controlos de volume.</span><span class="sxs-lookup"><span data-stu-id="14131-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="14131-113">Alguns oradores e aplicações têm os seus próprios controlos de volume; Talvez tenha que verificar todos para se certificar de que estão nos níveis certos.</span><span class="sxs-lookup"><span data-stu-id="14131-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="14131-114">Tente ligar-se utilizando uma porta USB diferente.</span><span class="sxs-lookup"><span data-stu-id="14131-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="14131-115">**Nota:** Lembre-se de que os altifalantes podem não funcionar quando os auscultadores estiverem ligados.</span><span class="sxs-lookup"><span data-stu-id="14131-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="14131-116">**Verificar Gestor de Dispositivos**</span><span class="sxs-lookup"><span data-stu-id="14131-116">**Check Device Manager**</span></span>

<span data-ttu-id="14131-117">Para garantir que os condutores estão atualizados:</span><span class="sxs-lookup"><span data-stu-id="14131-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="14131-118">Selecione **Iniciar,** digitar **Gestor de Dispositivos**e, em seguida, selecione Gestor de **Dispositivos** na lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="14131-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="14131-119">Em **comandos de som, vídeo e jogo,** selecione a sua placa de som, abra-a, selecione o separador **Driver** e selecione 'Controlador de **atualização**' .</span><span class="sxs-lookup"><span data-stu-id="14131-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="14131-120">**Nota:** Se o Windows não encontrar um novo controlador, procure um no site do fabricante do dispositivo e siga as suas instruções.</span><span class="sxs-lookup"><span data-stu-id="14131-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="14131-121">**Reinstalar o controlador**</span><span class="sxs-lookup"><span data-stu-id="14131-121">**Reinstall the driver**</span></span>

<span data-ttu-id="14131-122">Se não conseguir atualizar via Device Manager ou encontrar um novo controlador no site do fabricante, experimente estes passos:</span><span class="sxs-lookup"><span data-stu-id="14131-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="14131-123">No Gestor do Dispositivo, clique à direita (ou prima e segure) o controlador de áudio e selecione **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="14131-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="14131-124">Reiniciar o seu dispositivo e o Windows tentará reinstalar o controlador.</span><span class="sxs-lookup"><span data-stu-id="14131-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="14131-125">Se a reinstalação do controlador não funcionar, tente utilizar o controlador de áudio genérico que vem com o Windows.</span><span class="sxs-lookup"><span data-stu-id="14131-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="14131-126">No Gestor do Dispositivo, clique à direita (ou pressione e segure) o seu controlador de áudio > **Atualizar o software** > do controlador**Navegue no meu computador para** > o software do controlador**Deixe-me escolher de uma lista de controladores de dispositivos no meu computador,** selecione Dispositivo de Áudio de **Alta Definição,** selecione **Next**, e siga as instruções para instalá-lo.</span><span class="sxs-lookup"><span data-stu-id="14131-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
