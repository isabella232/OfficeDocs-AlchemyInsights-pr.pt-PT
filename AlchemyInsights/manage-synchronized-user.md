---
title: Gerir o utilizador sincronizado
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823978"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="eef28-102">Não é possível definir o endereço de e-mail primário, alterar atributos do utilizador ou remover/eliminar um utilizador sincronizado</span><span class="sxs-lookup"><span data-stu-id="eef28-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="eef28-103">Se a sincronização de diretórios estiver ativada para o seu ambiente, alguns atributos de utilizador ou objeto não podem ser alterados utilizando o centro de administração Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eef28-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="eef28-104">Para gerir totalmente os utilizadores sincronizados e todos os seus atributos, utilize os utilizadores de diretórios ativos locais e a consola de gestão de grupos (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="eef28-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="eef28-105">Em alternativa, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados utilizando a powershell, tal como mostrado nestes exemplos comuns:</span><span class="sxs-lookup"><span data-stu-id="eef28-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
