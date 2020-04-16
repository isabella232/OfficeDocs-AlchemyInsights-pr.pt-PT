---
title: Definir respostas automáticas numa caixa de correio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509512"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Definir respostas automáticas na caixa de correio de um utilizador

**Método 1**

1. Inicie sessão no portal do Office 365.

2. Aceda a **Utilizadores > Utilizadores ativos** (ou **Grupos > Caixas de correio partilhadas** se a definição for implementada numa caixa de correio partilhada).

3. Selecione um utilizador que tenha uma caixa de correio do Microsoft Exchange.

4. No menu de contexto à direita, aceda a **Definições de correio > Respostas automáticas** (se for uma caixa de correio partilhada, basta clicar em **Respostas automáticas** no menu de contexto).

**Método 2**

1. Inicie sessão no portal de administração do Office 365 com credenciais de administrador.

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
