---
title: Alterar endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756568"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Alterar endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams

Você pode alterar o endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams ao utilizar o [centro de administração do Microsoft 365](https://admin.microsoft.com/). Basta selecionar o grupo e selecionar @editar endereço de e-mail.

Também pode utilizar o seguinte comando EXO Windows PowerShell para alterar o endereço primário SMTP de um Microsoft 365 grupo/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplo: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
