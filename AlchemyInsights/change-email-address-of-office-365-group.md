---
title: Alterar o endereço de e-mail de um grupo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930740"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Alterar o endereço de e-mail de um grupo Microsoft 365

Pode alterar o endereço de e-mail de um grupo Microsoft 365 ao utilizar o centro de administração. Basta selecionar o grupo e selecionar @editar endereço de e-mail.

Também pode utilizar o seguinte comando EXO Windows PowerShell para alterar o endereço SMTP primário de um grupo Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exemplo: 

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
