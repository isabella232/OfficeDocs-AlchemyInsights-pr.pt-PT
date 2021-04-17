---
title: Problemas de resolução de problemas com a inscrição de dispositivos iOS no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823474"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problemas de resolução de problemas com a inscrição de dispositivos iOS no Microsoft Intune

Reveja os recursos listados abaixo para resolver o seu problema agora. 
  
Algumas mensagens de erro comuns e etapas de resolução:
  
- **Tampa do dispositivo alcançada** O utilizador tem mais dispositivos matriculados do que o limite do dispositivo. Reveja estes documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Este Serviço não é suportado. Sem Política de Inscrição:** O Serviço de Notificação de Push apple (APNS) precisa de ser configurado ou renovado. [Reveja este documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) para obter instruções sobre como fazê-lo. 
    
- **Tipo de licença de utilizador Inválido ou Nome de Utilizador Não Reconhecido:** O utilizador precisa de ser atribuído a uma licença Intune ou EMS. Reveja estes documentos para atribuir uma licença através [de: Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ou [portal Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Recursos adicionais para ajudar a resolver o seu problema:
  
1. Utilize [o Portal de Resolução de Problemas Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de inscrição. [Reveja este documento](https://docs.microsoft.com/intune/help-desk-operators) para mais detalhes. 
    
2. Consulte estes documentos para obter uma lista de erros comuns que impedem a inscrição e resoluções de cada um: [Guia de resolução de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento de Resolução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Saiba como inscrever dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

