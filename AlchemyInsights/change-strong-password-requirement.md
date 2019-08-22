---
title: Requisito de palavra-passe segura de alteração
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518770"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="c50a9-102">Requisito de palavra-passe segura de alteração</span><span class="sxs-lookup"><span data-stu-id="c50a9-102">Change strong password requirement</span></span>

<span data-ttu-id="c50a9-103">A Microsoft requer palavras-passe seguras por predefinição.</span><span class="sxs-lookup"><span data-stu-id="c50a9-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="c50a9-104">Utilizar o PowerShell, pode desactivar a palavras-passe seguras para utilizadores específicos com este comando:</span><span class="sxs-lookup"><span data-stu-id="c50a9-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="c50a9-105">*Conjunto-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="c50a9-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="c50a9-106">Mais informações sobre políticas de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="c50a9-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="c50a9-107">Como ligar ao Office 365. o com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="c50a9-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="c50a9-108">Mais informações sobre comandos do PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="c50a9-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)