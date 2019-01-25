---
title: Resolver problemas relacionados com a inscrição de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29484014"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Resolver problemas relacionados com a inscrição de dispositivos Android no Microsoft Intune

Reveja os recursos listados abaixo para resolver o problema agora.
  
Alguns problemas comuns e passos de resolução:
  
 **Dispositivo não encriptados erro no Portal da empresa:** Versões mais recentes do Android, particularmente começando v 7.0, exigem uma palavra-passe de arranque para se certificar de que o dispositivo está totalmente encriptado. São soluções comuns activar um pin de arranque ou encriptar totalmente o dispositivo. Reveja [Este documento](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para obter mais informações. 
  
 **Falham a verificação com o serviço de Intune ou como "Unhealthy" na consola de administração do Intune:** Alguns 4.4 Samsung e 5.5 dispositivos não podem verificar no serviço. Existem 3 soluções possíveis para este problema: 
  
1. Abra manualmente a aplicação de Portal da empresa de Intune, que iniciará automaticamente uma sincronização de dispositivo.
    
2. Actualize o dispositivo para Android 6.0 ou superior.
    
3. Desactive Gestor inteligentes Samsung da gestão do Portal da empresa de Intune. Reveja [Este documento](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para obter mais detalhes sobre estes problemas e resoluções. 
    
 **Tipo de licença de utilizador inválido** ou **erro de utilizador nome não reconhecido:** o utilizador tem de ser atribuída uma licença de Intune ou EMS. Reveja estes documentos para atribuir uma licença através de: centro Admin do Office ou Azure portal. 
  
Recursos adicionais para ajudar a resolver o problema:
  
1. Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) para obter mais detalhes. 
    
2. Reveja [Este documento](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) para uma lista de erros comuns que impedem a inscrição e resoluções para cada um. 
    
3. [Obter informações sobre como inscrever-se dispositivos Android no Intune da Microsoft](https://docs.microsoft.com/en-us/intune/android-enroll).
    

