---
title: Gerir utilizador sincronizado
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542011"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="9eb45-102">Não é possível definir o endereço de correio electrónico principal ou alterar atributos de utilizador</span><span class="sxs-lookup"><span data-stu-id="9eb45-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="9eb45-103">Se a sincronização de directório estiver activada para o seu ambiente, alguns atributos de utilizador ou objecto não podem ser alterados utilizando o Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9eb45-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="9eb45-104">Para gerir totalmente sincronizados utilizadores e os respectivos atributos, utilize o local active directory utilizadores e grupos consola de gestão (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="9eb45-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="9eb45-105">Em alternativa, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados utilizando powershell tal como indicado nestes exemplos comuns:</span><span class="sxs-lookup"><span data-stu-id="9eb45-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="9eb45-106">Conjunto-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9eb45-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="9eb45-107">Conjunto-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Utilizador de teste" - Apelido "Utilizador"-"Gestor" do título-departamento "H"</span><span class="sxs-lookup"><span data-stu-id="9eb45-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="9eb45-108">Remover-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="9eb45-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>