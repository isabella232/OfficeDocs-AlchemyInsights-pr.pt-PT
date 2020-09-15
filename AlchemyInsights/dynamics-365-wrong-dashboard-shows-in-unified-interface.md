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
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="8f2b9-102">Painel de instrumentos errado mostra na Interface Unificada Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="8f2b9-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="8f2b9-103">Existem várias razões pelas quais pode ver um painel diferente daquele que espera:</span><span class="sxs-lookup"><span data-stu-id="8f2b9-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="8f2b9-104">O utilizador definiu um painel de instrumentos predefinido do utilizador</span><span class="sxs-lookup"><span data-stu-id="8f2b9-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="8f2b9-105">Normalmente, é possível identificar um painel de instrumentos predefinido do utilizador se o botão **"Como Predefinido"** não aparecer na barra de comando do painel de instrumentos.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="8f2b9-106">O painel de instrumentos predefinido do utilizador irá sobrepor-se a todos os outros dashboards predefinidos, mesmo que o painel de instrumentos predefinido do utilizador não esteja na aplicação atual.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="8f2b9-107">Utilize a seguinte solução para desacorrentar o seu painel de instrumentos predefinido.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="8f2b9-108">Criar um novo painel pessoal.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="8f2b9-109">Desafine o novo painel de instrumentos como o padrão do utilizador.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="8f2b9-110">Apaga o painel.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="8f2b9-111">O painel de instrumentos está definido no mapa do site</span><span class="sxs-lookup"><span data-stu-id="8f2b9-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="8f2b9-112">Pode ter definido um dashboard padrão da organização selecionando um dashboard e escolhendo 'set As Default' em 'Personalizar o Sistema'.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="8f2b9-113">Mas o dashboard definido no sitemap designer terá precedência sobre este dashboard, se o utilizador tiver acesso ao mesmo.</span><span class="sxs-lookup"><span data-stu-id="8f2b9-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="8f2b9-114">Para que os utilizadores vejam o dashboard que definiu como o padrão da organização, pode:</span><span class="sxs-lookup"><span data-stu-id="8f2b9-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="8f2b9-115">Coloque o painel no mapa do site</span><span class="sxs-lookup"><span data-stu-id="8f2b9-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="8f2b9-116">Remova o acesso ao mapa de site definido para esses utilizadores</span><span class="sxs-lookup"><span data-stu-id="8f2b9-116">Remove access to the sitemap defined dashboard for those users</span></span>
