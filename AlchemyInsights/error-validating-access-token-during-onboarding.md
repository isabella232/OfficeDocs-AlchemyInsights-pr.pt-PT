---
title: Houve um erro validando o erro de acesso ao token durante a internação da Desktop Analytics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741244"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Houve um erro validando o erro de acesso ao token" durante a integração da Desktop Analytics

Esse erro é normalmente observado quando o token de autenticação expira. Normalmente, atualizar a página atualiza o token. No entanto, esse problema pode persistir se houver políticas de acesso condicional aplicadas à conta que está sendo usada na Desktop Analytics a bordo. Você pode revisar o AD Azure Sign In em logs no Portal Azure para ver se há alguma falha de login para a conta que está sendo usada para integração de Desktop Analytics.

Para obter mais informações sobre acesso condicional, visite o plano de sua implantação de [acesso condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)