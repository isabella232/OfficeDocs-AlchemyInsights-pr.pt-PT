---
title: Utilizar o Acesso Condicional com o Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005785"
---
# <a name="using-conditional-access-with-intune"></a>Utilizar o Acesso Condicional com o Intune

A utilização do Acesso Condicional com o Intune requer 3 passos:

- [Crie uma Política de Conformidade para definir as definições que têm de ser cumpridas antes de o dispositivo ser considerado conforme. Por exemplo, um dispositivo tem de ter um PIN de, pelo menos, 6 dígitos para que seja considerado conforme.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Criar uma Política de Acesso Condicional que defina que recursos estão a ser protegidos e que condições têm de ser cumpridas para aceder a esses recursos. Por exemplo, um dispositivo tem de estar em compatibilidade antes de aceder ao e-mail da empresa.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Certifique-se de que as Políticas de Conformidade e as Políticas de Acesso Condicional estão direccionais para os grupos de utilizadores pretendidos. Isto pode exigir a criação de grupos específicos de utilizadores no Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Saiba mais...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
