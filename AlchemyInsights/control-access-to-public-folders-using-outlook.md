---
title: Controlar o acesso às pastas públicas através do Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816751"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar o acesso às pastas públicas através do Outlook

Para controlar os utilizadores que podem aceder às pastas públicas através do Outlook:

1. Utilizar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Permitir que os utilizadores acedam às pastas públicas no Outlook  
$false: Impedir o acesso de utilizadores a pastas públicas no Outlook. Este é o valor predefinido.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: Este procedimento apenas pode controlar as ligações com o ambiente de trabalho do Outlook para clientes Windows. Os utilizadores podem continuar a aceder a pastas públicas com o OWA ou o Outlook para Mac.

Para obter mais informações, consulte [Ligações Controladas a Pastas Públicas no Outlook](https://aka.ms/controlpf).
