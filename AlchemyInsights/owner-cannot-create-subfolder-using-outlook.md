---
title: O proprietário não pode criar sub-pasta usando o Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836146"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>O proprietário não pode criar sub-pasta usando o Outlook

**Há um problema contínuo com os proprietários de pastas públicas que criam sub-dobradores usando o Outlook. A questão será resolvida em breve.**

Entretanto, utilize uma das seguintes soluções alternativas:

1. Use outlook para MAC para criar a sub-dobradeira, uma vez que o problema impacta apenas o Outlook para janelas de ambiente de trabalho (todas as versões)
2. Ter a administração criar a subpasta usando EXO Shell ou EAC
3. Altere a Caixa postal/Correio de Correio por defeitoPublicFoldermailbox no utilizador para outra caixa de correio que a caixa de correio de conteúdo para a pasta que causa problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Espere por uma hora, reinicie o cliente outlook