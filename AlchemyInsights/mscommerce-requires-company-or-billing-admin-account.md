---
title: Ligue-se ao módulo MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093612"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="29b82-102">MSCommerce requer uma conta de Administrador de Faturação ou Empresa</span><span class="sxs-lookup"><span data-stu-id="29b82-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="29b82-103">O módulo MSCommerce requer uma conta com privilégios de Administrador de Empresa ou Faturação.</span><span class="sxs-lookup"><span data-stu-id="29b82-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="29b82-104">Se estiver a receber o seguinte erro, terá de se reconectar com uma conta diferente.</span><span class="sxs-lookup"><span data-stu-id="29b82-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

<span data-ttu-id="29b82-105">Se a sua conta não tiver privilégios de Administrador de Empresa ou Faturação, contacte o seu Administrador de TI.</span><span class="sxs-lookup"><span data-stu-id="29b82-105">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
