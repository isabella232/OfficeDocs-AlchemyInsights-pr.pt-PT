---
title: Remova problemas com a inscrição Windows dispositivos na Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981052"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Remova problemas com a inscrição Windows dispositivos na Microsoft Intune

Reveja os recursos listados abaixo para resolver o seu problema agora.
  
Algumas mensagens de erro comuns e passos de resolução:
  
 **O software não pode ser instalado, 0x80cf4017:** O seu certificado de conta expirou. Transfira o pacote de software Cliente do PC na Consola do Administrador do Intune. Reveja esta documentação para obter mais informações.
  
 **Código de 0x801c0003:** O erro pode ocorrer nos seguintes cenários:
  
-  O utilizador tem mais dispositivos inscritos do que o limite de dispositivos. Reveja estes documentos [para remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Os utilizadores podem associar dispositivos ao Azure AD" está definido como "nenhum". Defina-a para todos ou selecione utilizadores. [Reveja esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obter mais informações.

-  O dispositivo já está inscrito por outro utilizador. Se for esse o caso, remova o dispositivo da consola do Azure Intune ou desenrole manualmente o dispositivo antes de tentar novamente.

-  O dispositivo está Windows 10 Home. Apenas os Windows 10 Pro, Educação e Enterprise podem aderir Azure Active Directory.

Recursos adicionais para ajudar a resolver o seu problema:
  
-  Utilize o Portal de Resolução de Problemas do [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. [Reveja este](https://docs.microsoft.com/intune/help-desk-operators) documento para obter mais detalhes.

-  Consulte estes documentos para obter uma lista de erros comuns que impedem a inscrição e resoluções de cada um: [Guia de resolução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento de Resolução de Problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Saiba como inscrever Windows dispositivos no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
