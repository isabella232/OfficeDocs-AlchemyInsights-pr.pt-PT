---
title: Problemas de resolução de problemas com a inscrição de dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708973"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="bd276-102">Problemas de resolução de problemas com a inscrição de dispositivos iOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bd276-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="bd276-103">Reveja os recursos listados abaixo para resolver o seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="bd276-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="bd276-104">Algumas mensagens de erro comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="bd276-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="bd276-105">**Tampa do dispositivo alcançada** O utilizador tem mais dispositivos matriculados do que o limite do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bd276-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="bd276-106">Reveja estes documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="bd276-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="bd276-107">**Este Serviço não é suportado. Sem Política de Inscrição:** O Serviço de Notificação de Push apple (APNS) precisa de ser configurado ou renovado.</span><span class="sxs-lookup"><span data-stu-id="bd276-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="bd276-108">[Reveja este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazê-lo.</span><span class="sxs-lookup"><span data-stu-id="bd276-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="bd276-109">**Tipo de licença de utilizador Inválido ou Nome de Utilizador Não Reconhecido:** O utilizador precisa de ser atribuído a uma licença Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="bd276-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bd276-110">Reveja estes documentos para atribuir uma licença através [de: Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ou [portal Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="bd276-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="bd276-111">Recursos adicionais para ajudar a resolver o seu problema:</span><span class="sxs-lookup"><span data-stu-id="bd276-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bd276-112">Utilize [o Portal de Resolução de Problemas Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de inscrição.</span><span class="sxs-lookup"><span data-stu-id="bd276-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bd276-113">[Reveja este documento](https://docs.microsoft.com/intune/help-desk-operators) para mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="bd276-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="bd276-114">Reveja estes documentos para obter uma lista de erros comuns que impeçam a inscrição e as resoluções para cada um: [Guia de resolução de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [doc de resolução de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bd276-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="bd276-115">[Saiba como inscrever dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="bd276-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

