---
title: Houve um erro a validar o erro do token de acesso durante o desktop Analytics no embarque
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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813699"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="b2d62-102">"Houve um erro a validar o erro do token de acesso" durante o desktop Analytics no embarque</span><span class="sxs-lookup"><span data-stu-id="b2d62-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="b2d62-103">Este erro é normalmente observado quando o token de autenticação expira.</span><span class="sxs-lookup"><span data-stu-id="b2d62-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="b2d62-104">Normalmente, refrescar a página refresca o símbolo.</span><span class="sxs-lookup"><span data-stu-id="b2d62-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="b2d62-105">No entanto, este problema pode persistir se existirem algumas políticas de Acesso Condicional aplicadas à conta que está a ser utilizada para o Desktop Analytics a bordo.</span><span class="sxs-lookup"><span data-stu-id="b2d62-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="b2d62-106">Pode rever o sinal AZure AD In registos no Portal Azure para ver se existem falhas de login na conta que estão a ser utilizadas para desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="b2d62-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="b2d62-107">Para mais informações sobre o Acesso Condicionado, visite [Plan a sua implementação de Acesso Condicional.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="b2d62-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>