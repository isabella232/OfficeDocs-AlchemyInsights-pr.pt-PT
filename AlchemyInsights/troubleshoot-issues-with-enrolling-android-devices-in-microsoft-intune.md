---
title: Remova problemas com a inscrição de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008089"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Remova problemas com a inscrição de dispositivos Android no Microsoft Intune

Reveja os recursos listados abaixo para resolver o seu problema agora.
  
Alguns problemas comuns e passos de resolução:
  
 **Erro de dispositivo que não está encriptado Portal da Empresa:** As versões mais recentes do Android, particularmente a partir do v7.0, necessitam de um código de seta de arranque para garantir que o dispositivo está totalmente encriptado. As soluções comuns são ativar um pin de arranque ou encriptar totalmente o dispositivo. [Reveja este](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) documento para obter mais informações.
  
 Os dispositivos não é apresentado com o serviço do Intune ou são apresentados como **"Inhealthy"** na consola do administrador do Intune: Alguns dispositivos Samsung 4.4 e 5.5 poderão não ter entrada do serviço. Existem 3 soluções possíveis para este problema:
  
1. Abra manualmente a aplicação Portal da Empresa do Intune, que iniciará automaticamente uma sincronização de dispositivos.

2. Atualize o dispositivo para o Android 6.0 ou superior.

3. Desativar o Samsung Smart Manager para gerir o Portal da Empresa do Intune. [Reveja este](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) documento para obter mais detalhes sobre estes problemas e resoluções.

 **Tipo de Licença de** Utilizador Inválido ou Erro de Nome de Utilizador Não **Reconhecido:** é necessário que o utilizador esteja atribuído a uma licença do Intune ou EMS. Reveja estes documentos para atribuir uma licença através Office centro de administração ou portal do Azure.
  
Recursos adicionais para ajudar a resolver o seu problema:
  
1. Utilize o Portal de Resolução de Problemas do [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas de inscrição comuns. [Reveja este](https://docs.microsoft.com/intune/help-desk-operators) documento para obter mais detalhes.

2. [Reveja este](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) documento para ver uma lista de erros comuns que impedem a inscrição e as resoluções de cada um.

3. [Saiba como inscrever dispositivos Android no Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
