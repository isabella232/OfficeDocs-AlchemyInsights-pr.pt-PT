---
title: Gerir Utilizador Sincronizado
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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114789"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Não é possível definir o endereço de e-mail principal, alterar atributos do utilizador ou remover/eliminar um utilizador sincronizado

Se a sincronização de diretórios estiver ativada para o seu ambiente, alguns atributos de utilizador ou objeto não podem ser alterados através da centro de administração do Microsoft 365.

Para gerir totalmente os utilizadores sincronizados e todos os respetivos atributos, utilize a consola de gestão de grupos e utilizadores do Active Directory local (adsiedit.msc).  

Em alternativa, pode alterar utilizadores individuais ou atributos de utilizadores sincronizados através do powershell, como é mostrado nestes exemplos comuns:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
