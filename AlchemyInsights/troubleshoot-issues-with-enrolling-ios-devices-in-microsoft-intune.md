---
title: Resolver problemas relacionados com a inscrição de dispositivos de iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658450"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="44174-102">Resolver problemas relacionados com a inscrição de dispositivos de iOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="44174-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="44174-103">Reveja os recursos listados abaixo para resolver o problema agora.</span><span class="sxs-lookup"><span data-stu-id="44174-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="44174-104">Algumas mensagens de erro comuns e passos de resolução:</span><span class="sxs-lookup"><span data-stu-id="44174-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="44174-p101">**Dispositivo Cap atingido** O utilizador tem mais dispositivos de inscritos que o limite do dispositivo. Reveja estes documentos para [Remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="44174-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="44174-p102">**Este serviço não é suportada. Nenhuma política de inscrição:** Apple Push notificação de serviço (APNS) tem de ser configurada ou renovado. Reveja [Este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazê-lo.</span><span class="sxs-lookup"><span data-stu-id="44174-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="44174-p103">**Inválido de tipo de licença do utilizador ou nome de utilizador não reconhecido:** O utilizador tem de ser atribuída uma licença de Intune ou EMS. Reveja estes documentos para atribuir uma licença através de: [Centro Admin do Office](https://docs.microsoft.com/intune/licenses-assign) ou [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="44174-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="44174-111">Recursos adicionais para ajudar a resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="44174-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="44174-p104">Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="44174-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="44174-114">Reveja estes documentos para uma lista de erros comuns que impedem a inscrição e resoluções para cada uma: [manual de resolução de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [documentos de resolução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="44174-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="44174-115">[Obter informações sobre como inscrever-se dispositivos iOS Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="44174-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

