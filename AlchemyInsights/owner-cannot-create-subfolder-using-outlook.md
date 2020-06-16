---
title: O proprietário não pode criar sub-pasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749141"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>O proprietário não pode criar sub-pasta usando o Outlook

**Há um problema contínuo com os proprietários de pastas públicas que criam sub-dobradores usando o Outlook. A questão será resolvida em breve.**

Entretanto, utilize uma das seguintes soluções alternativas:

1. Use outlook para MAC para criar a sub-dobradeira, uma vez que o problema impacta apenas o Outlook para janelas de ambiente de trabalho (todas as versões)
2. Ter a administração criar a subpasta usando EXO Shell ou EAC
3. Altere a Caixa postal/Correio de Correio por defeitoPublicFoldermailbox no utilizador para outra caixa de correio que a caixa de correio de conteúdo para a pasta que causa problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Espere por uma hora, reinicie o cliente outlook