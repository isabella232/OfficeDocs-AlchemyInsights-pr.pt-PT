---
title: Sincronização de senha de resolução de problemas
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732521"
---
# <a name="troubleshoot-password-synchronization"></a>Sincronização de senha de resolução de problemas

Para resolver problemas em que nenhuma palavra-passe é sincronizada com a versão 1.1.614.0 do Azure AD Connect:
  
1. Abra uma nova sessão do Windows PowerShell no seu servidor Azure AD Connect com a opção **Executar como Administrador.**

2. Executar **Política de execução de séries Remotamente Assinada** ou Política de Execução de **Conjuntos sem restrições**.

3. Inicie o assistente Azure AD Connect.

4. Navegue na página **De Tarefas Adicionais,** selecione **Troubleshoot**, e clique **em Next**.

5. Na página Deresolução de Problemas, clique em Lançar para iniciar o menu de resolução de **problemas** no PowerShell.

6. No menu principal, selecione **Troubleshoot Password Synchronization**.

7. No menu sub, selecione **Password Synchronization não funciona**de todo .

**Compreenda os resultados da tarefa de resolução de problemas**
  
A tarefa de resolução de problemas realiza as seguintes verificações:
  
- Valida que a funcionalidade de sincronização de palavras-passe está ativada para o seu inquilino Azure AD.

- Valida que o servidor Azure AD Connect não esteja em modo de encenação.

- Para cada conector ativo de diretório existente no local (que corresponde a uma floresta de Diretório Ativo existente):

- 
  - Valida que a função de sincronização da palavra-passe esteja ativada.

  - Pesquisas por eventos de batimentocardíaco de sincronização de palavras-passe nos registos do Windows Application Event.

  - Para cada domínio de Diretório Ativo sob o conector ative diretório no local:

  - Valida que o domínio é acessível a partir do servidor Azure AD Connect.

  - Valida que as contas de Serviços de Domínio de Diretório Ativo (AD DS) utilizadas pelo conector Ative Directory no local têm o nome de utilizador, palavra-passe e permissões corretas necessárias para a sincronização de palavras-passe.

Para obter mais ajuda na resolução de sincronização de palavras-passe, consulte a [sincronização da palavra-passe de Troubleshoot com a sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  