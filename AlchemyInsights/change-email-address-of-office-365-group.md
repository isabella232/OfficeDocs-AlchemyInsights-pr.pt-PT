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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819055"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Alterar o endereço de e-mail de um grupo Microsoft 365

Pode alterar o endereço de e-mail de um grupo Microsoft 365 ao utilizar o centro de administração. Basta selecionar o grupo e selecionar @editar endereço de e-mail.

Também pode utilizar o seguinte comando EXO Windows PowerShell para alterar o endereço SMTP primário de um grupo Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exemplo: 

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
