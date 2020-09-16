---
title: O proprietário não pode criar sub-pasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665729"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>O proprietário não pode criar sub-pasta usando o Outlook

**Há um problema contínuo com os proprietários de pastas públicas que criam sub-dobradores usando o Outlook. A questão será resolvida em breve.**

Entretanto, utilize uma das seguintes soluções alternativas:

1. Use outlook para MAC para criar a sub-dobradeira, uma vez que o problema impacta apenas o Outlook para janelas de ambiente de trabalho (todas as versões)
2. Ter a administração criar a subpasta usando EXO Shell ou EAC
3. Altere a Caixa postal/Correio de Correio por defeitoPublicFoldermailbox no utilizador para outra caixa de correio que a caixa de correio de conteúdo para a pasta que causa problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Espere por uma hora, reinicie o cliente outlook