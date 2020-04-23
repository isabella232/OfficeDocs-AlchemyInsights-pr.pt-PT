---
title: Problemas de resolução de problemas com a inscrição de dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736169"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemas de resolução de problemas com a inscrição de dispositivos iOS no Microsoft Intune

Reveja os recursos listados abaixo para resolver o seu problema agora. 
  
Algumas mensagens de erro comuns e passos de resolução:
  
- **Tampa do dispositivo alcançada** O utilizador tem mais dispositivos matriculados do que o limite do dispositivo. Reveja estes documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Este Serviço não é suportado. Sem política de inscrição:** O Serviço de Notificação push da Apple (APNS) precisa de ser configurado ou renovado. Reveja [este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazê-lo. 
    
- **Tipo de licença de utilizador Inválido ou Nome de Utilizador não reconhecido:** O utilizador precisa de ser atribuído a uma licença Intune ou EMS. Reveja estes documentos para atribuir uma licença através de: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ou [portal Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Recursos adicionais para ajudar a resolver o seu problema:
  
1. Utilize o Portal de Resolução de [Problemas Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de matrícula. Reveja [este documento](https://docs.microsoft.com/intune/help-desk-operators) para mais detalhes. 
    
2. Reveja estes documentos para obter uma lista de erros comuns que impeçam a inscrição e resoluções de cada um: Guia de resolução de [problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e doc de resolução de [problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Saiba como inscrever dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

