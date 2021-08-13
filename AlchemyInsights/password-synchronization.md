---
title: Password synchronization
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960846"
---
# <a name="password-synchronization"></a>Password synchronization

**A Sincronização de Hashs de Palavras-passe não funciona de todo**

Alguns problemas comuns que os clientes encontram quando a Sincronização de Hash de Palavras-passe não funciona são:

- A conta do Active Directory utilizada pelo Azure AD Ligação para comunicar com o Active Directory no local não tem permissão para **Replicar** Alterações ao Diretório e **Replicar** Alterações ao Diretório Todas as permissões, que são necessárias para a sincronização de palavras-passe – tem de corrigir este problema ao conceder estas permissões à conta do Active Directory.
- A sincronização de hashes de palavras-passe é desativada após um administrador alterar o método User Sign-In (Sincronização de Palavras-passe) para outra opção, como Federação com **O AD FS** no assistente do Azure AD Ligação – pode corrigir este problema ao reativar a funcionalidade de sincronização de hashes de palavras-passe no assistente de sincronização de hashes do Azure AD Ligação.  
- Problema de conectividade com o Active Directory no local. Por exemplo, alguns controladores de domínio não são acessíveis pelo Azure AD Ligação ou as portas necessárias são bloqueadas pela Firewall - Tem de corrigir este problema assegurando que a conectividade entre o servidor do Azure AD Ligação e o Active Directory no local funciona corretamente. [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)
- O servidor de Ligação do Azure AD está atualmente em modo de teste, o que fará com que o servidor não consiga encontrar hashes de palavras-passe - Para resolução de problemas, siga os passos descritos na secção Resolução de problemas de sincronização de palavras-passe com o [Azure AD Ligação sincronizado – não são sincronizadas](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)palavras-passe.

**A Sincronização de Hashs de Palavras-passe não funciona para alguns dos meus utilizadores**

1. Caso tenha reparado que o hash de palavra-passe não está a ser a ser syncing para um utilizador, utilize a tarefa de resolução de problemas no Azure AD Ligação para investigar e resolver o problema.  Efetue as seguintes tarefas:

    a. [Executar a tarefa de remoção de problemas no assistente](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Utilize o cmdlet de remoção de problemas para investigar o problema de síntese de hash da palavra-passe para uma utilização específica](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. O objeto do Utilizador do Active Directory no local está ativado para o Utilizador tem de alterar a **palavra-passe na próxima opção de início de** sessão. Quando esta opção está ativada, é atribuída ao utilizador uma palavra-passe temporária e ser-lhe-á pedido para alterar a palavra-passe no início de sessão seguinte. O Azure AD Ligação não sincroniza palavras-passe temporárias com o Azure AD.

Para resolver o problema acima, efetue uma das seguintes tarefas:

- Peça ao utilizador para entrar na aplicação no local (por exemplo, no Windows ambiente de trabalho) e alterar a palavra-passe. A nova palavra-passe será sincronizada com o Azure AD.
- Pedir a um administrador para atualizar a palavra-passe do utilizador sem ativar a opção O utilizador tem de alterar a palavra-passe no início de sessão seguinte e partilhar a nova palavra-passe com o utilizador.

3. O objeto do Utilizador do Active  Directory no local não está configurado corretamente para sincronização de objetos ou sincronização de palavras-passe. Para remoção deste problema, siga os passos descritos na remoção de problemas de sincronização de hashes de palavras-passe com o [Azure AD Ligação sincronização.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







