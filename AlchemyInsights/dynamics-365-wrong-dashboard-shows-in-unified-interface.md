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
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748409"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="d7c7d-102">Dashboard errado mostra na interface unificada Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d7c7d-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="d7c7d-103">Existem várias razões por que razão poderá ver um dashboard diferente daquele que espera:</span><span class="sxs-lookup"><span data-stu-id="d7c7d-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="d7c7d-104">O utilizador tiver definido um dashboard predefinido</span><span class="sxs-lookup"><span data-stu-id="d7c7d-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="d7c7d-105">Normalmente, consegue identificar um utilizador dashboard predefinido é definido se o botão **Predefinir** não mostrar na barra de comando de dashboard.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="d7c7d-106">O dashboard predefinido de utilizador irá substituir todos os outros dashboards predefinido, mesmo que o dashboard predefinido do utilizador não está a ser a aplicação actual.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="d7c7d-107">Utilize a seguinte solução alternativa para anular seu dashboard predefinido.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="d7c7d-108">Crie um novo dashboard pessoal.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="d7c7d-109">Defina esse novo dashboard como o predefinido pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="d7c7d-110">Elimine esse dashboard.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="d7c7d-111">O dashboard é definido no mapa do site</span><span class="sxs-lookup"><span data-stu-id="d7c7d-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="d7c7d-112">Pode ter definido um dashboard predefinido de organização, seleccionando um dashboard e escolher 'Predefinir' em 'Personalizar o sistema'.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="d7c7d-113">Mas o dashboard definido no designer do mapa do site terão precedência sobre este dashboard, se o utilizador tiver acesso à mesma.</span><span class="sxs-lookup"><span data-stu-id="d7c7d-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="d7c7d-114">Para os utilizadores, consulte o dashboard que definiu como a organização predefinida, pode:</span><span class="sxs-lookup"><span data-stu-id="d7c7d-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="d7c7d-115">Definir esse dashboard em mapa do site</span><span class="sxs-lookup"><span data-stu-id="d7c7d-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="d7c7d-116">Remover acesso ao dashboard de mapa do site definido para os utilizadores</span><span class="sxs-lookup"><span data-stu-id="d7c7d-116">Remove access to the sitemap defined dashboard for those users</span></span>
