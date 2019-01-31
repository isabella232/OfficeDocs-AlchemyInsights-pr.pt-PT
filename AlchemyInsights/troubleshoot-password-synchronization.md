---
title: Resolução de problemas de sincronização de palavra-passe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 589820c945fb20f00431655f9f53196e740bb38f
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655822"
---
# <a name="troubleshoot-password-synchronization"></a>Resolução de problemas de sincronização de palavra-passe

Para resolver problemas em que nenhuma palavra-passe é sincronizadas com Azure AD ligar versão 1.1.614.0 ou posterior:
  
1. Abra uma nova sessão do Windows PowerShell no servidor Azure AD ligar com a opção **Executar como administrador** . 
    
2. Executar **conjunto ExecutionPolicy RemoteSigned** ou **conjunto ExecutionPolicy ilimitado**. 
    
3. Inicie o Assistente de ligação de AD Azure.
    
4. Navegue para o * * tarefas adicionais * * página, seleccione * * resolução de problemas * * e clique em **seguinte**. 
    
5. Na página de resolução de problemas, clique em menu **Iniciar para iniciar a resolução de problemas** no PowerShell. 
    
6. No menu principal, seleccione a **Resolução de problemas de sincronização de palavra-passe**. 
    
7. No menu ' sub ', seleccione a **sincronização de palavra-passe não funciona em todos os**. 
    
 **Compreender os resultados da tarefa de resolução de problemas**
  
A tarefa de resolução de problemas efectua as seguintes verificações:
  
- Confirma que a funcionalidade de sincronização de palavra-passe está activada para o locatário Azure AD.
    
- Confirma que o servidor de Azure AD ligar não está no modo de teste.
    
- Para cada existentes no local conector do Active Directory (que corresponde a uma floresta existente do Active Directory):
    
- 
  - Confirma que a funcionalidade de sincronização de palavra-passe está activada.
    
  - Procura de eventos de heartbeat de sincronização de palavra-passe nos registos de eventos de aplicações do Windows.
    
  - Para cada domínio do Active Directory com o Active Directory connector no local:
    
  - Confirma que o domínio é acessível a partir do servidor Azure AD ligar.
    
  - Confirma-se de que as contas de serviços de domínio do Active Directory (AD DS) utilizadas pelo conector Active Directory no local tem o nome de utilizador correcto, palavra-passe e permissões necessárias para a sincronização de palavra-passe.
    
Para obter mais ajuda, resolução de problemas de sincronização de palavra-passe, consulte [sincronização de palavra-passe de resolução de problemas com sincronização Azure AD ligar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

