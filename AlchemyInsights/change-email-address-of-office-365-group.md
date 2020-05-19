---
title: Alterar endereço de e-mail de um grupo Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283257"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Alterar endereço de e-mail de um grupo Microsoft 365

Pode alterar o endereço de e-mail de um grupo Microsoft 365 utilizando o centro de administração. Basta selecionar o grupo e selecionar @edit endereço de e-mail.

Também pode utilizar o comando EXO PowerShell para alterar o endereço SMTP primário de um grupo Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Exemplo:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
