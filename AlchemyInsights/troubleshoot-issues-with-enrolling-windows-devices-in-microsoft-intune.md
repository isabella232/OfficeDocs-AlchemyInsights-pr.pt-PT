---
title: Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665843"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Resolver problemas relacionados com a inscrição de dispositivos do Windows no Microsoft Intune

Reveja os recursos listados abaixo para resolver o problema agora.
  
Algumas mensagens de erro comuns e passos de resolução:
  
 **Não é possível instalar o software, 0x80cf4017:** O certificado de conta expirou. Voltar a transferir o pacote de software de cliente de PC na consola de Admin de Intune. Reveja a documentação para obter mais informações.
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:
  
-  O utilizador tem mais dispositivos de inscritos que o limite do dispositivo. Reveja estes documentos para [Remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou [alterar o limite do dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Os utilizadores podem associar dispositivos a Azure AD" é definido para 'none'. Defina-o a todos ou seleccione os utilizadores. Reveja [a documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.

-  O dispositivo já está inscrito por outro utilizador. Se for esse o caso, remova o dispositivo da consola Azure Intune ou unenroll manualmente o dispositivo antes de tentar novamente.

-  O dispositivo for Windows 10 Home. Apenas Windows 10 Pro, da educação e SKUs de empresa, podem associar Azure Active Directory.

Recursos adicionais para ajudar a resolver o problema:
  
-  Utilize o [Portal de resolução de problemas de Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. Reveja [Este documento](https://docs.microsoft.com/intune/help-desk-operators) para obter mais detalhes.

-  Reveja estes documentos para uma lista de erros comuns que impedem a inscrição e resoluções para cada uma: [manual de resolução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [documentos de resolução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Obter informações sobre como inscrever-se os dispositivos no Intune do Microsoft Windows](https://docs.microsoft.com/intune/windows-enroll).
