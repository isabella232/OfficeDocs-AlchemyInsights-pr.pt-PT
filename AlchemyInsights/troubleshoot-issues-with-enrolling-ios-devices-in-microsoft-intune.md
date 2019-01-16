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
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306387"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Resolver problemas relacionados com a inscrição de dispositivos de iOS no Microsoft Intune

Reveja os recursos listados abaixo para resolver o problema agora. 
  
Algumas mensagens de erro comuns e passos de resolução:
  
- **Dispositivo Cap atingido** O utilizador tem mais dispositivos de inscritos que o limite do dispositivo. Reveja estes documentos para [Remover um dispositivo](https://docs.microsoft.com/en-us/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Este serviço não é suportada. Nenhuma política de inscrição:** Apple Push notificação de serviço (APNS) tem de ser configurada ou renovado. Reveja [Este documento](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazê-lo. 
    
- **Inválido de tipo de licença do utilizador ou nome de utilizador não reconhecido:** O utilizador tem de ser atribuída uma licença de Intune ou EMS. Reveja estes documentos para atribuir uma licença através de: [Centro Admin do Office](https://docs.microsoft.com/en-us/intune/licenses-assign) ou [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Recursos adicionais para ajudar a resolver o problema:
  
1. Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) para obter mais detalhes. 
    
2. Reveja estes documentos para uma lista de erros comuns que impedem a inscrição e resoluções para cada uma: [manual de resolução de problemas](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [documentos de resolução de problemas](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Obter informações sobre como inscrever-se dispositivos iOS Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

