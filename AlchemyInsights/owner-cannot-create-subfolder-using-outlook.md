---
title: O proprietário não pode criar subpa pasta utilizando Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063135"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>O proprietário não pode criar subpa pasta utilizando Outlook

**Existe um problema contínuo em que os proprietários de pastas públicas criam subpatas com o Outlook. O problema será corrigido em breve.**

Entretanto, utilize uma das seguintes sões:

1. Utilize Outlook para MAC para criar a subpase como o problema afeta apenas Outlook para janelas de ambiente de trabalho (todas as versões)
2. Fazer com que o administrador crie a subpasso através da Shell EXO ou do EAC
3. Alterar a caixa defaultPublicFolderMailbox/EffectivePublicFolderMailbox do utilizador para outra caixa de correio que não a Caixa de Correio de Conteúdo da pasta que está a causar o problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Aguarde por uma hora, reinicie o cliente do outlook