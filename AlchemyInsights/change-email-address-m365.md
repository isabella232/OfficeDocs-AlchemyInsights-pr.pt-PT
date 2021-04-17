---
title: Alterar endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819091"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Alterar endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams

Você pode alterar o endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams ao utilizar o [centro de administração do Microsoft 365](https://admin.microsoft.com/). Basta selecionar o grupo e selecionar @editar endereço de e-mail.

Também pode utilizar o seguinte comando EXO Windows PowerShell para alterar o endereço primário SMTP de um Microsoft 365 grupo/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplo: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
