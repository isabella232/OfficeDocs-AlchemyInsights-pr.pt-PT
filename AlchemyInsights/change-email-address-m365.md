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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="fbb7f-102">Alterar endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fbb7f-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="fbb7f-103">Você pode alterar o endereço de e-mail de um grupo Microsoft 365 ou Microsoft Teams ao utilizar o [centro de administração do Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="fbb7f-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="fbb7f-104">Basta selecionar o grupo e selecionar @editar endereço de e-mail.</span><span class="sxs-lookup"><span data-stu-id="fbb7f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="fbb7f-105">Também pode utilizar o seguinte comando EXO Windows PowerShell para alterar o endereço primário SMTP de um Microsoft 365 grupo/Teams:</span><span class="sxs-lookup"><span data-stu-id="fbb7f-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="fbb7f-106">Exemplo: </span><span class="sxs-lookup"><span data-stu-id="fbb7f-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
