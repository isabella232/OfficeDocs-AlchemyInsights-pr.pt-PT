---
title: Utilize as linhas de segurança Microsoft Intune para configurar dispositivos Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696378"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="5226a-102">Utilize as linhas de segurança Microsoft Intune para configurar dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="5226a-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="5226a-103">As linhas de segurança intune ajudam a proteger os utilizadores e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5226a-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="5226a-104">As linhas de base de segurança são os grupos pré-configurados das definições do Windows utilizados para aplicar um grupo conhecido de definições e valores predefinidos recomendados pelas equipas de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="5226a-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="5226a-105">Ao criar um perfil de base de segurança no Intune, cria-se um modelo que consiste em múltiplos perfis de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5226a-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="5226a-106">Quando implementa linhas de segurança para grupos de utilizadores ou dispositivos, as definições são aplicadas em dispositivos que funcionam nas versões windows 10 ou posteriores.</span><span class="sxs-lookup"><span data-stu-id="5226a-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="5226a-107">Por exemplo, a linha de base de segurança de gestão de dispositivos móveis da Microsoft (MDM) ativa automaticamente (1) o BitLocker para unidades amovíveis, (2) requer a palavra-passe para desbloquear um dispositivo e (3) desativa a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="5226a-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="5226a-108">Quando um valor predefinido não funciona para o seu ambiente, pode personalizar a linha de base para aplicar as definições de que necessita.</span><span class="sxs-lookup"><span data-stu-id="5226a-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="5226a-109">As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5226a-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="5226a-110">Seguem-se alguns benefícios desta funcionalidade:</span><span class="sxs-lookup"><span data-stu-id="5226a-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="5226a-111">Uma linha de base de segurança inclui as melhores práticas e recomendações para configurações que afetam a segurança.</span><span class="sxs-lookup"><span data-stu-id="5226a-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="5226a-112">Uma vez que a Intune é parceira da equipa de segurança do Windows que cria linhas de base para políticas de grupo, estas recomendações baseiam-se numa orientação sólida e numa vasta experiência.</span><span class="sxs-lookup"><span data-stu-id="5226a-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="5226a-113">Se é novo no Intune e não sabe por onde começar, então as linhas de segurança irão ajudá-lo a criar rapidamente e a implementar um perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="5226a-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="5226a-114">Se está a usar uma política de grupo, então migrar para Intune para fins de gestão é muito mais fácil com bases de segurança, porque estas linhas de base de segurança são incorporadas no Intune e incluem capacidades de ponta para a gestão.</span><span class="sxs-lookup"><span data-stu-id="5226a-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="5226a-115">Para obter mais informações, consulte [as linhas de base de segurança do Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e a [gestão de dispositivos Móveis.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="5226a-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>