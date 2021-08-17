---
title: Remova a sincronização de palavras-passe
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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105768"
---
# <a name="troubleshoot-password-synchronization"></a>Remova a sincronização de palavras-passe

Para refletir problemas de sincronização de palavras-passe, comece por utilizar esta tarefa de remoção de problemas do AAD Ligação para determinar o motivo pelo qual as palavras-passe não estão a ser sincronizadas. Para começar, vá a Gerir [a sincronização direta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Abra uma nova sessão Windows PowerShell sessão no seu servidor de Ligação Azure AD e selecione a opção **Executar como** Administrador.

2. Execute Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Unrestricted.

3. Inicie o assistente de Início de Ligação Azure AD.

4. Vá para a página Tarefas Adicionais > **Seguinte.**  >  

5. **Selecione** Iniciar para abrir o menu de remoção de problemas do PowerShell.

6. **Selecione Remoção da Sincronização de Palavras-passe**.

    Normalmente, o problema é que uma palavra-passe não é sincronizada para uma conta de utilizador específica.

    **Notas** A sincronização de palavras-passe falha se a última sincronização de palavras-passe com êxito tiver sido há algum tempo.

Para mais ajuda na remoção de problemas de sincronização de palavras-passe, consulte Remova a sincronização de hashes de palavras-passe com o [Azure AD e Ligação sincronização.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)