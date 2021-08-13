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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995633"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Alterar endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams

Você pode alterar o endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams ao utilizar o [centro de administração do Microsoft 365](https://admin.microsoft.com/). Basta selecionar o grupo e selecionar @editar endereço de e-mail.

Também pode utilizar o seguinte comando EXO Windows PowerShell para alterar o endereço primário SMTP de um Microsoft 365 grupo/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplo: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
