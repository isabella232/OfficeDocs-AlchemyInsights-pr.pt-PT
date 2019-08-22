---
title: Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559672"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="63b22-102">Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="63b22-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="63b22-103">Reveja os recursos listados abaixo para resolver o problema agora.</span><span class="sxs-lookup"><span data-stu-id="63b22-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="63b22-104">Algumas mensagens de erro comuns e passos de resolução:</span><span class="sxs-lookup"><span data-stu-id="63b22-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="63b22-105">**Não é possível instalar o software, 0x80cf4017:** O certificado de conta expirou.</span><span class="sxs-lookup"><span data-stu-id="63b22-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="63b22-106">Voltar a transferir o pacote de software de cliente de PC na consola de Admin de Intune.</span><span class="sxs-lookup"><span data-stu-id="63b22-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="63b22-107">Reveja a documentação para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="63b22-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="63b22-108">**Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="63b22-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="63b22-109">O utilizador tem mais dispositivos de inscritos que o limite do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63b22-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="63b22-110">Reveja estes documentos para [Remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="63b22-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="63b22-111">"Os utilizadores podem associar dispositivos a Azure AD" é definido para 'none'.</span><span class="sxs-lookup"><span data-stu-id="63b22-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="63b22-112">Defina-o a todos ou seleccione os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="63b22-112">Set it to all or select users.</span></span> <span data-ttu-id="63b22-113">Reveja [a documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="63b22-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="63b22-114">O dispositivo já está inscrito por outro utilizador.</span><span class="sxs-lookup"><span data-stu-id="63b22-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="63b22-115">Se for esse o caso, remova o dispositivo da consola Azure Intune ou unenroll manualmente o dispositivo antes de tentar novamente.</span><span class="sxs-lookup"><span data-stu-id="63b22-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="63b22-116">O dispositivo for Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="63b22-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="63b22-117">Apenas Windows 10 Pro, da educação e SKUs de empresa, podem associar Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="63b22-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="63b22-118">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="63b22-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="63b22-119">Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns.</span><span class="sxs-lookup"><span data-stu-id="63b22-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="63b22-120">Reveja [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="63b22-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="63b22-121">Reveja estes documentos para uma lista de erros comuns que impedem a inscrição e resoluções para cada uma: [manual de resolução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [documentos de resolução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="63b22-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="63b22-122">[Obter informações sobre como inscrever-se os dispositivos no Intune do Microsoft Windows](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="63b22-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
