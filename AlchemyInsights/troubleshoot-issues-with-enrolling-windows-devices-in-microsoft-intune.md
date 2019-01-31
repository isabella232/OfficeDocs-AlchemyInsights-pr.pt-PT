---
title: Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661567"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="f6f0b-102">Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f6f0b-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="f6f0b-103">Reveja os recursos listados abaixo para resolver o problema agora.</span><span class="sxs-lookup"><span data-stu-id="f6f0b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f6f0b-104">Algumas mensagens de erro comuns e passos de resolução:</span><span class="sxs-lookup"><span data-stu-id="f6f0b-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="f6f0b-p101">**Não é possível instalar o software, 0x80cf4017:** O certificado de conta expirou. Voltar a transferir o pacote de software de cliente de PC na consola de Admin de Intune. Reveja a documentação para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f6f0b-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="f6f0b-108">**Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="f6f0b-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="f6f0b-p102">O utilizador tem mais dispositivos de inscritos que o limite do dispositivo. Reveja estes documentos para [Remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f6f0b-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="f6f0b-p103">"Os utilizadores podem associar dispositivos a Azure AD" é definido para 'none'. Defina-o a todos ou seleccione os utilizadores. Reveja [a documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f6f0b-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="f6f0b-p104">O dispositivo já está inscrito por outro utilizador. Se for esse o caso, remova o dispositivo da consola Azure Intune ou unenroll manualmente o dispositivo antes de tentar novamente.</span><span class="sxs-lookup"><span data-stu-id="f6f0b-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="f6f0b-p105">O dispositivo for Windows 10 Home. Apenas Windows 10 Pro, da educação e SKUs de empresa, podem associar Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6f0b-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="f6f0b-118">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="f6f0b-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f6f0b-p106">Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="f6f0b-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f6f0b-121">Reveja estes documentos para uma lista de erros comuns que impedem a inscrição e resoluções para cada uma: [manual de resolução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [documentos de resolução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f6f0b-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="f6f0b-122">[Obter informações sobre como inscrever-se os dispositivos no Intune do Microsoft Windows](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="f6f0b-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

