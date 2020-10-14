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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Não é possível definir o endereço de e-mail primário, alterar atributos do utilizador ou remover/eliminar um utilizador sincronizado

Se a sincronização de diretórios estiver ativada para o seu ambiente, alguns atributos de utilizador ou objeto não podem ser alterados utilizando o centro de administração Microsoft 365.

Para gerir totalmente os utilizadores sincronizados e todos os seus atributos, utilize os utilizadores de diretórios ativos locais e a consola de gestão de grupos (adsiedit.msc).  

Em alternativa, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados utilizando a powershell, tal como mostrado nestes exemplos comuns:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
