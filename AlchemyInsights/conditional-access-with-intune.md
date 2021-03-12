---
title: Acesso Condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704797"
---
# <a name="conditional-access-with-intune"></a>Acesso Condicional com Intune

A utilização  **do Acesso Condicional**  com Intune requer 3 passos:

- Crie uma  **Política de Conformidade** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)para definir as definições que devem ser satisfeitas antes de o dispositivo ser considerado conforme. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado conforme.
- Crie uma **Política de Acesso Condicional**  que defina que recursos estão a ser protegidos e que condições devem ser satisfeitas para aceder a esses recursos.  [Por exemplo,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  um dispositivo deve ser compatível antes de aceder a e-mails corporativos.
- Certifique-se de que ambas as **políticas de conformidade**  e políticas de acesso  **condicional**  são direcionadas para os grupos de utilizadores pretendidos. Isto pode exigir a criação de grupos específicos de utilizadores no Azure Ative Directory.

**Links úteis:**

[Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Resolução de problemas CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de resolução de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Para proteger o Email (Exchange online) do acesso por dispositivos não conformes, ambos os documentos devem ser seguidos:

1. [Proteja o acesso de e-mail a partir de dispositivos que utilizem EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteja o acesso de e-mail a partir de dispositivos que usem clientes de autenticação moderna como o Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)