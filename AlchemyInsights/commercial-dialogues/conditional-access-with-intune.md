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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749259"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="b304e-102">Utilização de Acesso Condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="b304e-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="b304e-103">A utilização do Acesso Condicional com Intune requer 3 passos:</span><span class="sxs-lookup"><span data-stu-id="b304e-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="b304e-104">Crie uma Política de Conformidade para definir as definições que devem ser satisfeitas antes de o dispositivo ser considerado conforme. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado conforme.</span><span class="sxs-lookup"><span data-stu-id="b304e-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="b304e-105">Crie uma Política de Acesso Condicional que defina que recursos estão a ser protegidos e que condições devem ser satisfeitas para aceder a esses recursos. Por exemplo, um dispositivo deve ser compatível antes de aceder a e-mails corporativos.</span><span class="sxs-lookup"><span data-stu-id="b304e-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="b304e-106">Certifique-se de que ambas as políticas de conformidade e políticas de acesso condicional são direcionadas para os grupos de utilizadores pretendidos. Isto pode exigir a criação de grupos específicos de utilizadores no Azure Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="b304e-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b304e-107">Saiba mais...</span><span class="sxs-lookup"><span data-stu-id="b304e-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
