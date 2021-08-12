---
title: Ocorreu um erro ao validar um erro de token de acesso durante a Análise de Ambiente de Trabalho
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946626"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Erro "Ocorreu um erro ao validar um token de acesso" durante a itivação da Análise de Ambiente de Trabalho

Este erro é normalmente observado quando o token de autenticação expira. Normalmente, atualizar a página atualiza o token. No entanto, este problema pode persistir se existirem políticas de Acesso Condicional aplicadas à conta que está a ser utilizada na Análise de Ambiente de Trabalho no quadro. Pode rever os registos de Início de Sessão do Azure AD no Portal do Azure para ver se existem falhas de início de sessão na conta que está a ser utilizada para a itivação da Análise de Ambiente de Trabalho.

Para obter mais informações sobre o Acesso Condicional, aceda a [Planear a sua implementação de Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)