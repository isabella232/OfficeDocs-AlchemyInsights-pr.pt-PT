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
# <a name="unable-to-change-username"></a><span data-ttu-id="a312a-102">Não é possível alterar o Nome do Utilizador</span><span class="sxs-lookup"><span data-stu-id="a312a-102">Unable to change UserName</span></span>

<span data-ttu-id="a312a-103">Em alguns casos, as alterações da UPN (UserPrincipalName) não são propagadas para a nuvem.</span><span class="sxs-lookup"><span data-stu-id="a312a-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="a312a-104">Pode receber erros de validação no portal Do Office 365 ou não poderá alterar o nome de utilizador ou endereço de e-mail.</span><span class="sxs-lookup"><span data-stu-id="a312a-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="a312a-105">Para resolver este problema, desapasse manualmente o Nome Do Utilizador Com este comando PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a312a-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="a312a-106">**Exemplo: Mudar o nome de um utilizador**</span><span class="sxs-lookup"><span data-stu-id="a312a-106">**Example: Rename a user**</span></span>

<span data-ttu-id="a312a-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a312a-107">PowerShellCopy</span></span>

<span data-ttu-id="a312a-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" - NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="a312a-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="a312a-109">Este comando renomea davidc@contoso.com para davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="a312a-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="a312a-110">Para mais informações, consulte [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="a312a-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>