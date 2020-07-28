---
title: Não é possível alterar o Nome do Utilizador
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440302"
---
# <a name="unable-to-change-username"></a>Não é possível alterar o Nome do Utilizador

Em alguns casos, as alterações da UPN (UserPrincipalName) não são propagadas para a nuvem. Pode receber erros de validação no portal Do Office 365 ou não poderá alterar o nome de utilizador ou endereço de e-mail. Para resolver este problema, desapasse manualmente o Nome Do Utilizador Com este comando PowerShell.

**Exemplo: Mudar o nome de um utilizador**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" - NewUserPrincipalName "davidchew@contoso.com"

Este comando renomea davidc@contoso.com para davidchew@contoso.com.

Para mais informações, consulte [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).