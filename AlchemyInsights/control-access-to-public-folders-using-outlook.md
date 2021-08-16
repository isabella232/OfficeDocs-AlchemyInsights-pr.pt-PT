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
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032569"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlar o acesso às pastas públicas através do Outlook

Para controlar os utilizadores que podem aceder às pastas públicas através do Outlook:

1. Utilizar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Permitir que os utilizadores acedam às pastas públicas no Outlook  
$false: Impedir o acesso de utilizadores a pastas públicas no Outlook. Este é o valor predefinido.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: Este procedimento apenas pode controlar as ligações com o ambiente de trabalho do Outlook para clientes Windows. Os utilizadores podem continuar a aceder a pastas públicas com o OWA ou o Outlook para Mac.

Para obter mais informações, consulte [Ligações Controladas a Pastas Públicas no Outlook](https://aka.ms/controlpf).
