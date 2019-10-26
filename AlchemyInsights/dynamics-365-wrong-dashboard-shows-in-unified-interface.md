---
title: Dinâmica 365 - Mostras de painel errado na interface unificada dynamics 365
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528562"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Painel errado mostra na interface unificada dynamics 365

Há várias razões pelas quais você pode ver um painel diferente do que você espera:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O usuário definiu um painel padrão do usuário 

Normalmente, você pode identificar que um painel padrão do usuário é definido se o botão **Set As Default** não aparecer na barra de comando do painel. O painel padrão do usuário substituirá todos os outros painéis padrão, mesmo que o painel padrão do usuário não esteja no aplicativo atual.

Use a seguinte solução para desdefinir seu painel padrão.

1. Crie um novo painel pessoal.

2. Defina esse novo painel como o padrão do usuário.

3. Exclua esse painel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O painel está definido no sitemap

Você pode ter definido um painel padrão da organização selecionando um painel e escolhendo "Set As Default" em "Personalize o sistema". Mas o painel definido no designer do sitemap terá precedência sobre este painel, se o usuário tiver acesso a ele.

Para que os usuários vejam o painel que você definiu como padrão da organização, você também pode:

* Defina esse painel no mapa do site

* Remover o acesso ao painel definido pelo mapa do site para esses usuários
