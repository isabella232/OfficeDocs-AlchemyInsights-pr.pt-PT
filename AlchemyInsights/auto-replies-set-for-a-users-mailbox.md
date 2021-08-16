---
title: Definir respostas automáticas numa caixa de correio
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
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046619"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Definir respostas automáticas na caixa de correio de um utilizador

**Método 1**

1. Inicie sessão no portal Microsoft 365.

2. Aceda a **Utilizadores > Utilizadores ativos** (ou **Grupos > Caixas de correio partilhadas** se a definição for implementada numa caixa de correio partilhada).

3. Selecione um utilizador que tenha uma caixa de correio do Microsoft Exchange.

4. No menu de contexto à direita, aceda a **Definições de correio > Respostas automáticas** (se for uma caixa de correio partilhada, basta clicar em **Respostas automáticas** no menu de contexto).

**Método 2**

1. Inicie sessão no portal de administração do Microsoft 365 através de credenciais de administrador.

2. Expanda **Centros de Administração** e, em seguida, clique em **Exchange**.

3. Clique na imagem no canto superior direito, clique em **Outro Utilizador** e, em seguida, selecione a caixa de correio do utilizador que pretende alterar.

4. No lado esquerdo, selecione **Opções**, clique em **Organizar E-mail** e clique em **Respostas automáticas.**

**Método 3**

Execute o seguinte cmdlet no PowerShell do Exchange Online:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Para mais informações acerca deste cmdlet, consulte [Configurar MailboxAutoAnswerConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
