---
title: Utilização de Acesso Condicional com Intune
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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694710"
---
# <a name="using-conditional-access-with-intune"></a>Utilização de Acesso Condicional com Intune

A utilização do Acesso Condicional com Intune requer 3 passos:

- [Crie uma Política de Conformidade para definir as definições que devem ser satisfeitas antes de o dispositivo ser considerado conforme. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado conforme.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Crie uma Política de Acesso Condicional que defina que recursos estão a ser protegidos e que condições devem ser satisfeitas para aceder a esses recursos. Por exemplo, um dispositivo deve ser compatível antes de aceder a e-mails corporativos.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Certifique-se de que ambas as políticas de conformidade e políticas de acesso condicional são direcionadas para os grupos de utilizadores pretendidos. Isto pode exigir a criação de grupos específicos de utilizadores no Azure Ative Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Saiba mais...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
