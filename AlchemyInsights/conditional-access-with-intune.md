---
title: Acesso Condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931447"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c7208-102">Acesso Condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="c7208-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c7208-103">A utilização **do Acesso Condicional** com Intune requer 3 passos:</span><span class="sxs-lookup"><span data-stu-id="c7208-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="c7208-104">Crie uma **Política de Conformidade** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)para definir as definições que devem ser satisfeitas antes de o dispositivo ser considerado conforme.</span><span class="sxs-lookup"><span data-stu-id="c7208-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c7208-105">Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado conforme.</span><span class="sxs-lookup"><span data-stu-id="c7208-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="c7208-106">Crie uma **Política de Acesso Condicional** que defina que recursos estão a ser protegidos e que condições devem ser satisfeitas para aceder a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="c7208-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="c7208-107">[Por exemplo,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) um dispositivo deve ser compatível antes de aceder a e-mails corporativos.</span><span class="sxs-lookup"><span data-stu-id="c7208-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="c7208-108">Certifique-se de que ambas as **políticas de conformidade** e políticas de acesso **condicional** são direcionadas para os grupos de utilizadores pretendidos.</span><span class="sxs-lookup"><span data-stu-id="c7208-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="c7208-109">Isto pode exigir a criação de grupos específicos de utilizadores no Azure Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="c7208-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="c7208-110">**Links úteis:**</span><span class="sxs-lookup"><span data-stu-id="c7208-110">**Helpful links:**</span></span>

[<span data-ttu-id="c7208-111">Visão geral da conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7208-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="c7208-112">Resolução de problemas CA</span><span class="sxs-lookup"><span data-stu-id="c7208-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c7208-113">Política de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="c7208-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="c7208-114">Para proteger o Email (Exchange online) do acesso por dispositivos não conformes, ambos os documentos devem ser seguidos:</span><span class="sxs-lookup"><span data-stu-id="c7208-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="c7208-115">Proteja o acesso de e-mail a partir de dispositivos que utilizem EAS</span><span class="sxs-lookup"><span data-stu-id="c7208-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="c7208-116">Proteja o acesso de e-mail a partir de dispositivos que usem clientes de autenticação moderna como o Outlook</span><span class="sxs-lookup"><span data-stu-id="c7208-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)