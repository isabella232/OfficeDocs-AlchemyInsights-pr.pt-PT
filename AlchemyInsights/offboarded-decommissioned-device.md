---
title: Problemas com a remoção de um dispositivo offboarded ou desmissionado do Inventário de Dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564345"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="d8a09-102">Problemas com a remoção de um dispositivo offboarded ou desmissionado do Inventário de Dispositivos</span><span class="sxs-lookup"><span data-stu-id="d8a09-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="d8a09-103">O Microsoft Defender para Pontos Finais não permite atualmente a remoção manual do registo do dispositivo de um dispositivo offboarded ou desmissionado do Inventário de Dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d8a09-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="d8a09-104">Por questões de segurança, o dispositivo permanece no portal como um registo histórico durante até 180 dias.</span><span class="sxs-lookup"><span data-stu-id="d8a09-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="d8a09-105">No entanto, os dados do dispositivo são retidos de acordo com o período de retenção configurado.</span><span class="sxs-lookup"><span data-stu-id="d8a09-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="d8a09-106">**Nota:** Um dispositivo offboarded ou desativado muda automaticamente para o estado **Inativo** após sete dias.</span><span class="sxs-lookup"><span data-stu-id="d8a09-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="d8a09-107">Além disso, os dispositivos que não estão ativos nos últimos 30 dias não são fatorizadas nos dados que refletem a pontuação de exposição Gestão de Vulnerabilidades e Ameaças da sua organização ou a Pontuação de Segurança da Microsoft para Dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d8a09-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="d8a09-108">Se ainda não quiser ver determinados dispositivos na vista Inventário de Dispositivos, experimente colocar uma etiqueta de dispositivo para filtrar o dispositivo des descomplicado a partir da vista Inventário de Dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d8a09-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="d8a09-109">Para mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="d8a09-109">For more information, see:</span></span>

[<span data-ttu-id="d8a09-110">Dispositivos offboard do serviço Microsoft Defender para Endpoint</span><span class="sxs-lookup"><span data-stu-id="d8a09-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="d8a09-111">Pontuação de exposição Gestão de Vulnerabilidades e Ameaças</span><span class="sxs-lookup"><span data-stu-id="d8a09-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="d8a09-112">Corrigir sensores desalojáveis no Microsoft Defender para Endpoint</span><span class="sxs-lookup"><span data-stu-id="d8a09-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="d8a09-113">Como utilizar a etiquetação de forma eficaz (Parte 1)</span><span class="sxs-lookup"><span data-stu-id="d8a09-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="d8a09-114">Como utilizar a etiquetação de forma eficaz (Parte 2)</span><span class="sxs-lookup"><span data-stu-id="d8a09-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="d8a09-115">Como utilizar a etiquetação de forma eficaz (Parte 3)</span><span class="sxs-lookup"><span data-stu-id="d8a09-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




