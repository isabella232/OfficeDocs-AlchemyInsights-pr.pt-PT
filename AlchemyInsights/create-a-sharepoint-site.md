---
title: Criar um site sharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770866"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="8ec93-102">Criar um site sharePoint</span><span class="sxs-lookup"><span data-stu-id="8ec93-102">Create a SharePoint site</span></span>

<span data-ttu-id="8ec93-103">Crie ou gere a partir de [Sites Ativos](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) no SharePoint Admin Center.</span><span class="sxs-lookup"><span data-stu-id="8ec93-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="8ec93-104">Para mais informações, consulte [Gerir sites no novo centro de administração do SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="8ec93-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="8ec93-105">Dicas:</span><span class="sxs-lookup"><span data-stu-id="8ec93-105">Tips:</span></span>

- <span data-ttu-id="8ec93-106">Não **é possível** criar um site com a mesma URL de um site existente.</span><span class="sxs-lookup"><span data-stu-id="8ec93-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="8ec93-107">Se apagou um site e pretende reutilizar o URL, é possível que o site apagado ainda exista em [sites Apagados](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="8ec93-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="8ec93-108">O site terá de ser permanentemente eliminado para reutilizar o URL.</span><span class="sxs-lookup"><span data-stu-id="8ec93-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="8ec93-109">Para remover completamente um site com Powershell, consulte o exemplo de [remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="8ec93-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="8ec93-110">Alguns utilizadores podem não ser capazes de criar um site.</span><span class="sxs-lookup"><span data-stu-id="8ec93-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="8ec93-111">Ver Gerir a criação do [site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="8ec93-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="8ec93-112">É possível que o site apareça preso na **Criação** mais tempo do que o esperado.</span><span class="sxs-lookup"><span data-stu-id="8ec93-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="8ec93-113">Se passaram mais de 24 horas desde que viu este problema pela primeira vez, por favor, faça um bilhete de apoio.</span><span class="sxs-lookup"><span data-stu-id="8ec93-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8ec93-114">Em muitos casos, já estamos a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="8ec93-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8ec93-115">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="8ec93-115">Please give us at least 24 hours to complete a solution.</span></span>
