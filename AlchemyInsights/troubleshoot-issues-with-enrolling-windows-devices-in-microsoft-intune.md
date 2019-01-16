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
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306184"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune

Reveja os recursos listados abaixo para resolver o problema agora. 
  
Algumas mensagens de erro comuns e passos de resolução:
  
 **Não é possível instalar o software, 0x80cf4017:** O certificado de conta expirou. Voltar a transferir o pacote de software de cliente de PC na consola de Admin de Intune. Reveja a documentação para obter mais informações. 
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários: 
  
1. O utilizador tem mais dispositivos de inscritos que o limite do dispositivo. Reveja estes documentos para [Remover um dispositivo](https://docs.microsoft.com/en-us/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Os utilizadores podem associar dispositivos a Azure AD" é definido para 'none'. Defina-o a todos ou seleccione os utilizadores. Reveja [a documentação](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações. 
    
3. O dispositivo já está inscrito por outro utilizador. Se for esse o caso, remova o dispositivo da consola Azure Intune ou unenroll manualmente o dispositivo antes de tentar novamente.
    
4. O dispositivo for Windows 10 Home. Apenas Windows 10 Pro, da educação e SKUs de empresa, podem associar Azure Active Directory.
    
Recursos adicionais para ajudar a resolver o problema:
  
1. Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) para obter mais detalhes. 
    
2. Reveja estes documentos para uma lista de erros comuns que impedem a inscrição e resoluções para cada uma: [manual de resolução de problemas](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [documentos de resolução de problemas](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Obter informações sobre como inscrever-se os dispositivos no Intune do Microsoft Windows](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

