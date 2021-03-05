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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482042"
---
# <a name="password-synchronization"></a>Password synchronization

**A sincronização de hash de palavra-passe não funciona de todo**

Algumas questões comuns que os clientes encontram quando a Sincronização de Password Hash não funciona são:

- A conta ative directory utilizada pelo Azure AD Connect para comunicar com o Ative Directory no local não é concedida Alterações de **Diretório de Replica** e **Alterações de Diretório de Replicatos,** que são necessárias para sincronização de palavras-passe - É necessário corrigi-lo concedendo estas permissões à conta ative Directory.
- A sincronização de hash de palavra-passe é desativada depois de um administrador ter alterado o método de Sign-In do Utilizador da Sincronização de **Passwords** para outra opção, como **a Federação com AD FS** no assistente Ad Connect Azure - Pode corrigi-lo, reativando a função de **sincronização de hash de palavra-passe** no assistente Ad Connect Azure.
- Problema de conectividade com o Ative Directory no local. Por exemplo, alguns controladores de domínio não estão [acessíveis](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) pelo Azure AD Connect, ou as portas necessárias são bloqueadas pelo Firewall - É necessário corrigi-lo garantindo que a conectividade entre o servidor AZURE AD Connect e o Ative Directory funciona corretamente.
- O servidor AD Connect Azure está atualmente em modo de fase, o que resultará na falta de acesso do servidor às hashes da palavra-passe - Para resolver o problema, siga os passos descritos na secção [Sincronização de palavras-passe de resolução de problemas com sincronização Azure AD Connect - Não há palavras-passe sincronizadas](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**A sincronização de hash de palavra-passe não funciona para alguns dos meus utilizadores**

1. Se notou que o hash da palavra-passe não está a sincronizar um utilizador, utilize a tarefa **de resolução de problemas** no Azure AD Connect para investigar e resolver o problema. Executar as seguintes tarefas:

    a. [Executar a tarefa de resolução de problemas no assistente](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Use o cmdlet de resolução de problemas para investigar o problema de sincronização de haxixe de palavra-passe para uma utilização específica](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. O objeto de utilizador ative directy no local está ativado para **o Utilizador deve alterar a palavra-passe na próxima** opção de início de sposição. Quando esta opção estiver ativada, o utilizador é atribuído a uma senha temporária e será solicitado a alterar a palavra-passe no próximo início de sessão. O Azure AD Connect não sincroniza palavras-passe temporárias para o Azure AD.

Para resolver a questão acima, execute qualquer uma das seguintes tarefas:

- Peça ao utilizador para iniciar sôms na aplicação no local (por exemplo, Windows Desktop) e altere a palavra-passe. A nova palavra-passe será sincronizada com a Azure AD.
- Tenha um administrador a atualizar a palavra-passe do utilizador sem permitir a opção O Utilizador deve alterar a **palavra-passe no próximo início de sê-lo** e partilhar a nova palavra-passe com o utilizador.

3. O objeto de utilizador ative directory no local não está **corretamente configurado** para sincronização de objetos ou sincronização de palavras-passe. Para resolver este problema, siga os passos descritos na [sincronização de hash de palavra-passe de resolução de problemas com a sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







