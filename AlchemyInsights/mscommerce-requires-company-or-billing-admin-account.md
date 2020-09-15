---
title: Ligue-se ao módulo MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702626"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce requer uma conta de Administrador de Empresa ou Faturação

O módulo MSCommerce requer uma conta com privilégios da Empresa ou do Administrador de Faturação. Se estiver a receber o seguinte erro, terá de voltar a ligar-se a uma conta diferente.

*ErrorMessage - O servidor remoto devolveu um erro: (403) Proibido. ErrorDetails - Em C:\Ficheiros de programa\WindowsPowerShell\Módulos\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Falhou em voltar a tentar ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoriaInfo : Não Específico: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Totalmente QualificadoErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Se a sua conta não tiver privilégios de Empresa ou Administrador de Faturação, contacte o seu Administrador de TI.
