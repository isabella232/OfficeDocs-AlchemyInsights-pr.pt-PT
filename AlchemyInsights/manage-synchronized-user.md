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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777688"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Não é possível definir o endereço de e-mail primário, alterar atributos do utilizador ou remover/eliminar um utilizador sincronizado

Se a sincronização de diretórios estiver ativada para o seu ambiente, alguns atributos de utilizador ou objeto não podem ser alterados utilizando o centro de administração Microsoft 365.

Para gerir totalmente os utilizadores sincronizados e todos os seus atributos, utilize os utilizadores de diretórios ativos locais e a consola de gestão de grupos (adsiedit.msc).  

Em alternativa, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados utilizando a powershell, tal como mostrado nestes exemplos comuns: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
