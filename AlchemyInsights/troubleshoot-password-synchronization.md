---
title: Sincronização de palavras-passe de resolução de problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387888"
---
# <a name="troubleshoot-password-synchronization"></a>Sincronização de palavras-passe de resolução de problemas

Para resolver problemas de sincronização de palavras-passe, comece por utilizar esta tarefa de resolução de problemas do AAD Connect para determinar por que razão as palavras-passe não estão a sincronizar. Para começar, vá para [Gerir a sincronização direta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Abra uma nova sessão Windows PowerShell no seu servidor Azure AD Connect e selecione a opção **Executar como Administrador.**

2. Executar Set-ExecuçãoPolítica RemoteSigned ou Set-ExecutionPolicy Sem restrições.

3. Inicie o assistente Azure AD Connect.

4. Aceda à página Tarefas Adicionais > **Resolução de Problemas**  >  **Em seguida**.

5. Selecione **Lançamento** para abrir o menu de resolução de problemas powerShell.

6. Selecione **A sincronização da palavra-passe de resolução de problemas**.

    O problema é que uma palavra-passe não é sincronizada para uma conta de utilizador específica.

    **Notas** A sincronização da palavra-passe falha se a última sincronização de senhas bem sucedidas foi há algum tempo.

Para obter mais ajuda para resolver problemas na sincronização da palavra-passe, consulte [a sincronização de hash de resolução de palavras-passe com sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).