---
title: Utilizar Microsoft Intune de base de segurança para configurar Windows 10 dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793893"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="b5c61-102">Utilizar Microsoft Intune de base de segurança para configurar Windows 10 dispositivos</span><span class="sxs-lookup"><span data-stu-id="b5c61-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="b5c61-103">As linhas de base de segurança do Intune ajudam a proteger os utilizadores e os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b5c61-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="b5c61-104">As linhas de base de Windows são grupos pré-configurados e configurados para aplicar um grupo conhecido de definições e valores predefinidos recomendados pelas equipas de segurança relevantes.</span><span class="sxs-lookup"><span data-stu-id="b5c61-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="b5c61-105">Ao criar um perfil de linha de base de segurança no Intune, cria um modelo que consiste em múltiplos perfis de configuração de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b5c61-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="b5c61-106">Ao implementar linhas de base de segurança em grupos de utilizadores ou dispositivos, as definições são aplicadas a dispositivos que são executados Windows 10 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="b5c61-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="b5c61-107">Por exemplo, a linha de base de segurança da gestão de dispositivos móveis (MDM) da Microsoft ativa automaticamente o BitLocker em unidades amovíveis, requer a palavra-passe para desbloquear um dispositivo e desativa a autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="b5c61-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="b5c61-108">Quando um valor predefinido não funcionar no seu ambiente, pode personalizar a linha base para aplicar as definições de que precisa.</span><span class="sxs-lookup"><span data-stu-id="b5c61-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="b5c61-109">As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro ponto a ponto no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b5c61-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="b5c61-110">Uma linha base de segurança inclui as práticas recomendadas e recomendações para definições que afetam a segurança.</span><span class="sxs-lookup"><span data-stu-id="b5c61-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="b5c61-111">O Intune tem parcerias com Windows equipa de segurança do Intune que cria linhas de base para políticas de grupo, pelo que estas recomendações baseiam-se em orientações sólidas e numa experiência extensa.</span><span class="sxs-lookup"><span data-stu-id="b5c61-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="b5c61-112">Se é novo no Intune e não sabe por onde começar, as linhas de base de segurança ajudam-no a criar e a implementar rapidamente um perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="b5c61-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="b5c61-113">Se utiliza atualmente uma política de grupo, é muito mais fácil migrar para o Intune para fins de gestão com linhas de base de segurança, uma vez que estão incorporadas no Intune e incluem funcionalidades de gestão de margem superior.</span><span class="sxs-lookup"><span data-stu-id="b5c61-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="b5c61-114">Para saber mais, consulte o Windows [de base de segurança e a gestão](/windows/security/threat-protection/windows-security-baselines) de [dispositivos móveis.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="b5c61-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

