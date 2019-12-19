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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="20c0f-102">"Houve um erro validando o erro de acesso ao token" durante a integração da Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="20c0f-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="20c0f-103">Esse erro é normalmente observado quando o token de autenticação expira.</span><span class="sxs-lookup"><span data-stu-id="20c0f-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="20c0f-104">Normalmente, atualizar a página atualiza o token.</span><span class="sxs-lookup"><span data-stu-id="20c0f-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="20c0f-105">No entanto, esse problema pode persistir se houver políticas de acesso condicional aplicadas à conta que está sendo usada na Desktop Analytics a bordo.</span><span class="sxs-lookup"><span data-stu-id="20c0f-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="20c0f-106">Você pode revisar o AD Azure Sign In em logs no Portal Azure para ver se há alguma falha de login para a conta que está sendo usada para integração de Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="20c0f-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="20c0f-107">Para obter mais informações sobre acesso condicional, visite o plano de sua implantação de [acesso condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="20c0f-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>