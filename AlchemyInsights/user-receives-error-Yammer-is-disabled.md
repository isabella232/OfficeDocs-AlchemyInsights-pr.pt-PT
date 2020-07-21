---
title: Utilizador recebe erro AADSTS7000112 Yammer está desativado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198375"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Utilizador recebe erro AADSTS7000112 Yammer está desativado

Se receber o erro "AADSTS7000112: Aplicação '0000005-0000-0ff1-ce00-0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000-000-0ff1-0000000000000000000000000000000 Um administrador pode ter desativado o diretor de serviço para bloquear o acesso ao Yammer.

A desativação do diretor de serviço não é recomendada e pode causar problemas adicionais. Para obter mais informações sobre a abordagem suportada para bloquear o acesso do utilizador ao Yammer, consulte [Desligue o acesso do Yammer aos utilizadores da Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Para corrigir este problema no Portal Azure e restaurar o acesso do utilizador ao Yammer:

1.  Abra a página do Diretório Ativo Azure e selecione **aplicações Enterprise** em **Manage** no painel de navegação esquerdo.
3.  Digite **Office 365 Yammer** na caixa de pesquisa e selecione o nome da aplicação para abrir as definições.
4.  Selecione **Propriedades** em **Manage** no painel de navegação esquerdo.
5.  Descreva o valor do **Yes** **Enabled para que os utilizadores se inscrevam?** **Save**
6.  Inscreva-se no Yammer de novo. Talvez precise de limpar os biscoitos.

Em alternativa, executar comandos PowerShell para definir o valor. Para mais informações, consulte ["Desculpe, mas estamos com dificuldades em inscrevê-lo" quando clicar no azulejo Yammer no Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 