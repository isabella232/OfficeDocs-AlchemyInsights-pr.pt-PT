---
title: Definir respostas automáticas na caixa de correio de um utilizador
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506528"
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

    Set-MailboxAutoReplyConfiguration

Para mais informações acerca deste cmdlet, consulte [Configurar MailboxAutoAnswerConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
