---
title: Remova problemas com a inscrição de dispositivos iOS no Microsoft Intune
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
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047987"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Remova problemas com a inscrição de dispositivos iOS no Microsoft Intune

Reveja os recursos listados abaixo para resolver o seu problema agora. 
  
Algumas mensagens de erro comuns e passos de resolução:
  
- **Limite de dispositivos Atingido** O utilizador tem mais dispositivos inscritos do que o limite de dispositivos. Reveja estes documentos [para remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Este Serviço não é suportado. Sem Política de Inscrição: o Serviço** de Notificações Push (APNS) da Apple tem de ser configurado ou renovado. [Reveja este](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) documento para obter instruções sobre como fazê-lo. 
    
- **Tipo de Licença de Utilizador Inválido ou Nome de Utilizador Não Reconhecido:** É necessário que seja atribuída ao utilizador uma licença do Intune ou EMS. Reveja estes documentos para atribuir uma licença através do Office [de Administração ou](https://docs.microsoft.com/intune/licenses-assign) do portal do [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Recursos adicionais para ajudar a resolver o seu problema:
  
1. Utilize o Portal de Resolução de Problemas do [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. [Reveja este](https://docs.microsoft.com/intune/help-desk-operators) documento para obter mais detalhes. 
    
2. Consulte estes documentos para obter uma lista de erros comuns que impedem a inscrição e resoluções de cada um: [Guia de resolução de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento de Resolução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Saiba como inscrever dispositivos iOS no Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

