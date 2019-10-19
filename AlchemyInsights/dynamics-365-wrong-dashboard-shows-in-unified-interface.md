---
title: Dynamics 365-mostra de Dashboard errado no Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528562"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>O painel incorreto mostra na interface unificada do Dynamics 365

Há várias razões pelas quais você pode ver um painel diferente daquele que você espera:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O usuário definiu um painel padrão do usuário 

Normalmente, você pode identificar um painel padrão do usuário é definido se o botão **definir como padrão** não aparecer na barra de comandos do Dashboard. O painel padrão do usuário substituirá todos os outros painéis padrão, mesmo que o painel padrão do usuário não esteja no aplicativo atual.

Use a seguinte solução alternativa para desdefinir seu painel padrão.

1. Crie um novo Dashboard pessoal.

2. Defina esse novo Dashboard como o padrão do usuário.

3. Exclua esse painel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O Dashboard é definido no sitemap

Você pode ter definido um painel padrão da organização selecionando um Dashboard e escolhendo ' definir como padrão ' em ' Personalizar o sistema '. Mas o Dashboard definido no designer do sitemap terá precedência sobre este Dashboard, se o usuário tiver acesso a ele.

Para que os usuários vejam o painel que você definiu como o padrão da organização, você pode:

* Definir esse Dashboard no sitemap

* Remover o acesso ao Dashboard definido pelo sitemap para esses usuários
