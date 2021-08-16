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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996641"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook não é possível ligar a pastas públicas

Se o acesso a pastas públicas não estiver a funcionar para alguns utilizadores, experimente o seguinte:

Ligação exO PowerShell e configure o parâmetro DefaultPublicFolderMailbox na conta do utilizador do problema para corresponder ao parâmetro numa conta de utilizador que funciona.

Exemplo:

Get-Mailbox TrabalharUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Aguarde pelo menos uma hora para que a alteração entre em vigor.

Se o problema permanecer, siga este [procedimento para](https://aka.ms/pfcte) remoção de problemas de acesso a pastas públicas utilizando Outlook.
 
**Para controlar quais os utilizadores que podem aceder a pastas públicas através Outlook:**

1.  Utilize Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false  
      
    $true: Permitir que os utilizadores acedam às pastas públicas no Outlook  
      
    $false: Impedir o acesso de utilizadores a pastas públicas no Outlook. Este é o valor predefinido.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControlar $true   
      
**Nota** Este procedimento pode controlar as ligações apenas com o Outlook ambiente de trabalho para Windows clientes. Um utilizador pode continuar a aceder a pastas públicas através do OWA ou do Outlook para Mac.
 
Para mais informações, consulte Anunciar o Suporte de Ligações Controladas para Pastas Públicas [no Outlook.](https://aka.ms/controlpf)