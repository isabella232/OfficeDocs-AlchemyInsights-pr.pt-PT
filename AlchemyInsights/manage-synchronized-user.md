---
title: Gerir o Utilizador Sincronizado
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407361"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="04448-102">Incapaz de definir o endereço de e-mail primário, alterar atributos do utilizador ou remover/eliminar um utilizador sincronizado</span><span class="sxs-lookup"><span data-stu-id="04448-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="04448-103">Se a sincronização do diretório estiver ativada para o seu ambiente, alguns atributos de utilizador ou objeto não podem ser alterados utilizando o centro de administração da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="04448-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="04448-104">Para gerir totalmente os utilizadores sincronizados e todos os seus atributos, utilize os utilizadores de diretórios ativos locais e a consola de gestão de grupos (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="04448-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="04448-105">Alternativamente, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados usando powershell, como mostrado nestes exemplos comuns:</span><span class="sxs-lookup"><span data-stu-id="04448-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
