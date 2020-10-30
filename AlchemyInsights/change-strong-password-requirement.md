---
title: Alterar requisito de senha forte
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804434"
---
# <a name="change-strong-password-requirement"></a>Alterar forte exigência de senha

A Microsoft requer senhas fortes por defeito.

Utilizando o PowerShell, pode desativar palavras-passe fortes para utilizadores específicos com estes comandos:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Para desativar palavras-passe fortes para todos os utilizadores, utilize:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Mais informações sobre a política de senhas](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Como ligar-se ao Microsoft 365 com o PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mais informações sobre comandos PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
