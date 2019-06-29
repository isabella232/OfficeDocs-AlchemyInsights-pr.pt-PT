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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380516"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Não é possível definir o endereço de correio electrónico principal ou alterar atributos de utilizador

Se a sincronização de directório estiver activada para o ambiente de alguns atributos de utilizador ou objecto não podem ser alterados utilizando o Centro de administração.
Para gerir totalmente sincronizados utilizadores e os respectivos atributos, utilize o local active directory utilizadores e grupos consola de gestão (Adsiedit. msc).  

Em alternativa, pode alterar utilizadores individuais ou atributos para utilizadores sincronizados utilizando powershell tal como indicado nestes exemplos comuns: 
- Conjunto-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Conjunto-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Utilizador de teste" - Apelido "Utilizador"-"Gestor" do título-departamento "H"
- Remover-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com