---
title: Estado do sensor de verificação do Ponto Final do Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676340"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="dfe91-102">Estado do sensor de verificação do Ponto Final do Defender</span><span class="sxs-lookup"><span data-stu-id="dfe91-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="dfe91-103">O **mosaico Dispositivos com** problemas de sensor encontra-se no dashboard Operações de Segurança.</span><span class="sxs-lookup"><span data-stu-id="dfe91-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="dfe91-104">Este mtilo fornece informações sobre a capacidade de um dispositivo individual fornecer dados de sensor e comunicar com o serviço Defender para Pontos Finais.</span><span class="sxs-lookup"><span data-stu-id="dfe91-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="dfe91-105">Reporta quantos dispositivos necessitam de atenção e ajuda-o a identificar dispositivos problemáticos e a tomar medidas para corrigir problemas conhecidos.</span><span class="sxs-lookup"><span data-stu-id="dfe91-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="dfe91-106">Dois indicadores de estado no mosaico fornecem informações sobre o número de dispositivos que não comunicam corretamente ao serviço:</span><span class="sxs-lookup"><span data-stu-id="dfe91-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="dfe91-107">**Configurado inde forma erradamente** Os dispositivos que podem estar parcialmente a comunicar dados do sensor ao Defender para serviço de Pontos Finais e podem ter erros de configuração que precisam de ser corrigidos.</span><span class="sxs-lookup"><span data-stu-id="dfe91-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="dfe91-108">**Inativo** Dispositivos que deixaram de comunicar com o Defender para serviço de Pontos Finais durante mais de sete dias no último mês.</span><span class="sxs-lookup"><span data-stu-id="dfe91-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="dfe91-109">Ao clicar em qualquer um dos grupos, é direcionado para a lista Dispositivos, filtrado de acordo com as suas opções.</span><span class="sxs-lookup"><span data-stu-id="dfe91-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="dfe91-110">Na lista de Dispositivos, pode filtrar a lista do estado de saúde pelo seguinte estado:</span><span class="sxs-lookup"><span data-stu-id="dfe91-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="dfe91-111">**Ativo** Dispositivos que comunicam ativamente ao serviço do Defender para Pontos Finais.</span><span class="sxs-lookup"><span data-stu-id="dfe91-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="dfe91-112">**Configurado inde forma erradamente** Os dispositivos que podem estar parcialmente a comunicar dados do sensor ao Defender para serviço de Pontos Finais, mas que têm erros de configuração que têm de ser corrigidos.</span><span class="sxs-lookup"><span data-stu-id="dfe91-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="dfe91-113">Os dispositivos mal configurados podem ter um ou uma combinação dos seguintes problemas:</span><span class="sxs-lookup"><span data-stu-id="dfe91-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="dfe91-114">Sem dados do sensor – os dispositivos deixaram de enviar dados do sensor.</span><span class="sxs-lookup"><span data-stu-id="dfe91-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="dfe91-115">Os alertas limitados podem ser ativados a partir do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dfe91-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="dfe91-116">Comunicações com deficiências - a capacidade de comunicar com dispositivos é prejudicada.</span><span class="sxs-lookup"><span data-stu-id="dfe91-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="dfe91-117">Enviar ficheiros para uma análise aprofundada, bloquear ficheiros, isolar o dispositivo da rede e outras ações que exijam comunicação com o dispositivo poderá não funcionar.</span><span class="sxs-lookup"><span data-stu-id="dfe91-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="dfe91-118">**Inativo** Dispositivos que deixaram de comunicar com o Serviço de Pontos Finais do Defender.</span><span class="sxs-lookup"><span data-stu-id="dfe91-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="dfe91-119">Pode transferir a lista completa no formato CSV com a funcionalidade Exportar.</span><span class="sxs-lookup"><span data-stu-id="dfe91-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="dfe91-120">Para obter mais informações, consulte [Verificar o estado de funcionamento do sensor no Microsoft Defender para Endpoint.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="dfe91-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="dfe91-121">Para obter mais informações sobre o que fez com que um dispositivo se encontrasse inativo ou mal configurado, consulte Corrigir sensores não em mau estado de funcionamento no [Microsoft Defender para o Endpoint.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="dfe91-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
