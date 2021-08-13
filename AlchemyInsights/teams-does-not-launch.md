---
title: Teams não inicia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813355"
---
# <a name="teams-doesnt-launch"></a>Teams não inicia

Se tentar abrir o Microsoft Teams mas este nunca é iniciado, experimente o seguinte:

1. Navegue até **%appdata%\Microsoft\Teams**.
1. Elimine o conteúdo da pasta.
1. Reinicie o computador e tente iniciar o Teams.

Poderá ter de reinstalar o Teams. Para reinstalar:

1. Desinstale o Teams através do Painel de Controlo.
1. Navegue até **%appdata%\Microsoft\Teams\Cache da Aplicação.**
1. Elimine o conteúdo da pasta.
1. Navegue até **%appdata%\Microsoft\teams\Cache.**
1. Elimine o conteúdo da pasta.
1. Reinicie o computador e, em seguida, transfira e instale o Teams.

Se pretende executar um diagnóstico no seu inquilino para um utilizador específico que não consegue iniciar a sua conta, comece uma nova pesquisa com a palavra-chave **TeamsUserUnableToSignIn** e siga as instruções.