---
title: Inventário de dispositivos intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667889"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="7cdeb-102">Inventário de dispositivos intune</span><span class="sxs-lookup"><span data-stu-id="7cdeb-102">Intune Device Inventory</span></span>

<span data-ttu-id="7cdeb-103">A lâmina devices fornece ao administrador informações sobre os dispositivos sob gestão no Intune por cada dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="7cdeb-104">As informações apresentadas incluem: Hardware, aplicações descobertas, estado de conformidade do dispositivo e estado de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="7cdeb-105">Os dados de inventário para hardware e aplicações descobertas são recolhidos num ciclo de sete dias.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="7cdeb-106">As aplicações e elementos específicos de hardware reportados diferem consoante o sistema operativo do dispositivo e se o dispositivo é de propriedade pessoal ou corporativa.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="7cdeb-107">Para mais informações, [consulte os detalhes do dispositivo no Intune.](https://docs.microsoft.com/intune/device-inventory)</span><span class="sxs-lookup"><span data-stu-id="7cdeb-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="7cdeb-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="7cdeb-108">**FAQ**</span></span>

<span data-ttu-id="7cdeb-109">P: Não estou a receber uma lista completa de aplicações presentes em dispositivos Windows matriculados no Intune.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="7cdeb-110">Porque não?</span><span class="sxs-lookup"><span data-stu-id="7cdeb-110">Why not?</span></span>

<span data-ttu-id="7cdeb-111">R: Neste momento, apenas aplicações modernas estão listadas para computadores Windows 10 que são identificados como dispositivos corporativos.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="7cdeb-112">A Intune não recolhe informações sobre as aplicações Win32 instaladas nestes dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="7cdeb-113">P: Por que os números de telefone não são recolhidos de todos os dispositivos?</span><span class="sxs-lookup"><span data-stu-id="7cdeb-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="7cdeb-114">R: Os telefones categorizados como dispositivos corporativos no Intune não são identificados com o seu número de telefone completo quando, por exemplo, você executou um relatório de inventário de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="7cdeb-115">Os números de telefone do dispositivo Bring-you são sempre parcialmente mascarados com asteriscos (\*\*\*\*), e mostram apenas os últimos quatro dígitos.</span><span class="sxs-lookup"><span data-stu-id="7cdeb-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>