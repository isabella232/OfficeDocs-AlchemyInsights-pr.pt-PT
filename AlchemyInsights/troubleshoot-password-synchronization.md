---
title: Sincronização de palavras-passe de resolução de problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664937"
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