---
title: Acesso Condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069723"
---
# <a name="conditional-access-with-intune"></a>Acesso Condicional com o Intune

A  **utilização do Acesso Condicional**  com o Intune requer 3 passos:

- Crie **uma Política de** Conformidade ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir as definições que têm de ser cumpridas antes de o dispositivo ser considerado conforme. Por exemplo, um dispositivo tem de ter um PIN de, pelo menos, 6 dígitos para que seja considerado conforme.
- Criar uma **Política de Acesso Condicional**  que defina que recursos estão a ser protegidos e que condições têm de ser cumpridas para aceder a esses recursos.  [Por exemplo, um](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  dispositivo tem de estar em compatibilidade antes de aceder ao e-mail da empresa.
- Certifique-se **de que as**  Políticas de Conformidade e as  **Políticas**  de Acesso Condicional estão direccionais para os grupos de utilizadores pretendidos. Isto pode exigir a criação de grupos específicos de utilizadores no Azure Active Directory.

**Ligações úteis:**

[Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Remoção de Problemas da AC](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de remoção de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Para proteger o E-mail (Exchange online) contra o acesso através de dispositivos nãocomplientes, ambos os documentos têm de ser seguidos:

1. [Proteger o acesso ao e-mail de dispositivos com o EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteger o acesso ao e-mail de dispositivos através de clientes de autenticação moderna, como Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)