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
ms.openlocfilehash: 10ef2e8fa7c564d53177a52136eb48cd709e5c55
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158519"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce requer uma conta de Administrador de Faturação ou Empresa

O módulo MSCommerce requer uma conta com privilégios de Administrador de Empresa ou Faturação. Se estiver a receber o seguinte erro, terá de se reconectar com uma conta diferente.

*ErrorMessage - O servidor remoto devolveu um erro: (403) Proibido. ErrorDetails - Em C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoriaInfo : Não Especificado: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ ErrorId totalmente qualificado : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Se a sua conta não tiver privilégios de Administrador de Empresa ou Faturação, contacte o seu Administrador de TI.
