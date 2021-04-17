---
title: Ligue-se ao módulo MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829747"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce requer uma conta de Administrador de Empresa ou Faturação

O módulo MSCommerce requer uma conta com privilégios da Empresa ou do Administrador de Faturação. Se estiver a receber o seguinte erro, terá de voltar a ligar-se a uma conta diferente.

*ErrorMessage - O servidor remoto devolveu um erro: (403) Proibido. ErrorDetails - Em C:\Ficheiros de programa\WindowsPowerShell\Módulos\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Falhou em voltar a tentar ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoriaInfo : Não Específico: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Totalmente QualificadoErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Se a sua conta não tiver privilégios de Empresa ou Administrador de Faturação, contacte o seu Administrador de TI.
