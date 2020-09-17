---
title: Houve um erro a validar o erro do token de acesso durante o desktop Analytics no embarque
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783562"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Houve um erro a validar o erro do token de acesso" durante o desktop Analytics no embarque

Este erro é normalmente observado quando o token de autenticação expira. Normalmente, refrescar a página refresca o símbolo. No entanto, este problema pode persistir se existirem algumas políticas de Acesso Condicional aplicadas à conta que está a ser utilizada para o Desktop Analytics a bordo. Pode rever o sinal AZure AD In registos no Portal Azure para ver se existem falhas de login na conta que estão a ser utilizadas para desktop Analytics.

Para mais informações sobre o Acesso Condicionado, visite [Plan a sua implementação de Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)