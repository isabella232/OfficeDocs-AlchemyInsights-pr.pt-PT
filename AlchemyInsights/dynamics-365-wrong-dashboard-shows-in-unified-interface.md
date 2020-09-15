---
title: Dinâmica 365 - Dashboard Errado Mostra em Dinâmica 365 Interface Unificada
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711286"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Painel de instrumentos errado mostra na Interface Unificada Dynamics 365

Existem várias razões pelas quais pode ver um painel diferente daquele que espera:

## <a name="the-user-has-set-a-user-default-dashboard"></a>O utilizador definiu um painel de instrumentos predefinido do utilizador 

Normalmente, é possível identificar um painel de instrumentos predefinido do utilizador se o botão **"Como Predefinido"** não aparecer na barra de comando do painel de instrumentos. O painel de instrumentos predefinido do utilizador irá sobrepor-se a todos os outros dashboards predefinidos, mesmo que o painel de instrumentos predefinido do utilizador não esteja na aplicação atual.

Utilize a seguinte solução para desacorrentar o seu painel de instrumentos predefinido.

1. Criar um novo painel pessoal.

2. Desafine o novo painel de instrumentos como o padrão do utilizador.

3. Apaga o painel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>O painel de instrumentos está definido no mapa do site

Pode ter definido um dashboard padrão da organização selecionando um dashboard e escolhendo 'set As Default' em 'Personalizar o Sistema'. Mas o dashboard definido no sitemap designer terá precedência sobre este dashboard, se o utilizador tiver acesso ao mesmo.

Para que os utilizadores vejam o dashboard que definiu como o padrão da organização, pode:

* Coloque o painel no mapa do site

* Remova o acesso ao mapa de site definido para esses utilizadores
