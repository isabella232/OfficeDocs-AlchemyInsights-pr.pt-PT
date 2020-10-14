---
title: Gerir o utilizador sincronizado
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451411"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="4eabf-102">Não é possível definir o endereço de e-mail primário, alterar atributos do utilizador ou remover/eliminar um utilizador sincronizado</span><span class="sxs-lookup"><span data-stu-id="4eabf-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="4eabf-103">Se a sincronização de diretórios estiver ativada para o seu ambiente, alguns atributos de utilizador ou objeto não podem ser alterados utilizando o centro de administração Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4eabf-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="4eabf-104">Para gerir totalmente os utilizadores sincronizados e todos os seus atributos, utilize os utilizadores de diretórios ativos locais e a consola de gestão de grupos (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="4eabf-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="4eabf-105">Em alternativa, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados utilizando a powershell, tal como mostrado nestes exemplos comuns:</span><span class="sxs-lookup"><span data-stu-id="4eabf-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
