---
title: Não é possível acessar pastas públicas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959505"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>O Outlook não pode se conectar a pastas públicas

Se o acesso público da pasta não está funcionando para poucos usuários, tente o seguinte:

Conecte-se ao EXO PowerShell e configure o DefaultPublicFolderMailbox na conta do usuário do problema para combinar uma em uma conta de usuário que trabalha.

Exemplo:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<valor de comando anterior>

Espere pelo menos uma hora para que a mudança entre em vigor.