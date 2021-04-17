---
title: Não é possível aceder a pastas públicas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819523"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook não pode ligar-se a pastas públicas

Se o acesso a pastas públicas não estiver a funcionar para alguns utilizadores, experimente o seguinte:

Ligue-se ao EXO PowerShell e configuure o parâmetro DefaultPublicFolderMailbox na conta de utilizador do problema para corresponder ao parâmetro numa conta de utilizador de trabalho.

Exemplo:

| de Get-Mailbox WorkingUser ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Espere pelo menos uma hora para a mudança fazer efeito.

Se o problema se mantiver, por favor siga [este procedimento](https://aka.ms/pfcte) para resolver problemas de acesso a pastas públicas usando o Outlook.
 
**Para controlar quais os utilizadores que podem aceder a pastas públicas utilizando o Outlook:**

1.  Utilize Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true: Permitir aos utilizadores aceder a pastas públicas no Outlook  
      
    $false: Impedir o acesso do utilizador a pastas públicas no Outlook. This is the default value.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Nota** Este procedimento só pode controlar as ligações com o desktop do Outlook para os clientes Windows. Um utilizador pode continuar a aceder a pastas públicas utilizando OWA ou Outlook for Mac.
 
Para obter mais informações, consulte [o Anúncio de Suporte para Ligações Controladas a Pastas Públicas no Outlook](https://aka.ms/controlpf).