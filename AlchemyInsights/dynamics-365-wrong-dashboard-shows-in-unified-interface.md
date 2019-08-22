---
title: Dynamics 365 - Dashboard errado mostra na Interface unificada Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528562"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dashboard errado mostra na interface unificada Dynamics 365

Existem várias razões por que razão poderá ver um dashboard diferente daquele que espera:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O utilizador tiver definido um dashboard predefinido 

Normalmente, consegue identificar um utilizador dashboard predefinido é definido se o botão **Predefinir** não mostrar na barra de comando de dashboard. O dashboard predefinido de utilizador irá substituir todos os outros dashboards predefinido, mesmo que o dashboard predefinido do utilizador não está a ser a aplicação actual.

Utilize a seguinte solução alternativa para anular seu dashboard predefinido.

1. Crie um novo dashboard pessoal.

2. Defina esse novo dashboard como o predefinido pelo utilizador.

3. Elimine esse dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O dashboard é definido no mapa do site

Pode ter definido um dashboard predefinido de organização, seleccionando um dashboard e escolher 'Predefinir' em 'Personalizar o sistema'. Mas o dashboard definido no designer do mapa do site terão precedência sobre este dashboard, se o utilizador tiver acesso à mesma.

Para os utilizadores, consulte o dashboard que definiu como a organização predefinida, pode:

* Definir esse dashboard em mapa do site

* Remover acesso ao dashboard de mapa do site definido para os utilizadores
