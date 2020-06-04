---
title: Problemas de resolução de problemas com a inscrição de dispositivos Windows no Microsoft Intune
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665843"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problemas de resolução de problemas com a inscrição de dispositivos Windows no Microsoft Intune

Reveja os recursos listados abaixo para resolver o seu problema agora.
  
Algumas mensagens de erro comuns e etapas de resolução:
  
 **O software não pode ser instalado, 0x80cf4017:** O seu certificado de conta expirou. Re-descarregue o pacote de software do Cliente PC na Consola Intune Admin. Reveja esta documentação para mais informações.
  
 **Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:
  
-  O utilizador tem mais dispositivos matriculados do que o limite do dispositivo. Reveja estes documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Os utilizadores podem juntar-se a dispositivos para Azure AD" está definido para "nenhum". Desacione-o a todos ou selecione os utilizadores. [Reveja esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para mais informações.

-  O dispositivo já está matriculado por outro utilizador. Se for esse o caso, retire o dispositivo da consola Azure Intune ou desative manualmente o dispositivo antes de voltar a tentar.

-  O dispositivo é o Windows 10 Home. Apenas o Windows 10 Pro, Education and Enterprise SKUs pode juntar-se ao Azure Ative Directory.

Recursos adicionais para ajudar a resolver o seu problema:
  
-  Utilize [o Portal de Resolução de Problemas Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de inscrição. [Reveja este documento](https://docs.microsoft.com/intune/help-desk-operators) para mais detalhes.

-  Reveja estes documentos para obter uma lista de erros comuns que impeçam a inscrição e as resoluções para cada um: [Guia de resolução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [doc de resolução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saiba como inscrever dispositivos Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
