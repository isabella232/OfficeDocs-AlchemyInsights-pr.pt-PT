---
title: Dynamics 365 – Dashboard Errado Mostra na Interface Unificada do Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101493"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>O dashboard errado é mostrado na interface unificada do Dynamics 365

Existem vários motivos pelos quais pode ver um dashboard diferente do esperado:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O utilizador tiver definido um dashboard predefinido do utilizador 

Normalmente, pode identificar o dashboard predefinido do utilizador se o botão Predefinido não aparecer na barra de comandos do dashboard.  O dashboard predefinido do utilizador irá predefinir todos os outros dashboards predefinido, mesmo que o dashboard predefinido do utilizador não se encontrar na aplicação atual.

Utilize a seguinte forma de resolver o seu dashboard predefinido.

1. Crie um novo dashboard pessoal.

2. Defina esse novo dashboard como a predefinição do utilizador.

3. Elimine esse dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O dashboard está definido noap do site

Pode ter definido um dashboard predefinido da organização ao selecionar um dashboard e selecionar "Predefinir" em "Personalizar o Sistema". Mas o dashboard definido no designer do sitemap terá precedência sobre este dashboard, se o utilizador tiver acesso ao mesmo.

Para que os utilizadores vejam o dashboard que predefinido para a organização, pode:

* Definir esse dashboard no sitemap

* Remover o acesso ao dashboard definido do site para esses utilizadores
