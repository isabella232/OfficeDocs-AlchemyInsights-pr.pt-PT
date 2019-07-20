---
title: Criar um site SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802977"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f6bbd-102">Criar um site SharePoint</span><span class="sxs-lookup"><span data-stu-id="f6bbd-102">Create a SharePoint site</span></span>

<span data-ttu-id="f6bbd-103">Pode ver o seguinte para obter informações sobre a criação de sites do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="f6bbd-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="f6bbd-104">[Gerir sites no novo Centro de administração do SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): obter informações sobre opções de criação de site, incluindo como criar um site clássico ou um site de equipas que não inclui um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="f6bbd-105">[Criar um site de equipa do SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Aprenda a criar um site de equipa.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="f6bbd-106">[Criar um site de comunicação no SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Aprenda a criar um site de comunicações.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="f6bbd-107">[Gerir sites no novo Centro de administração do SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Aprenda a criar um site clássico ou um site de equipa que não inclui um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Sugestões]
> - <span data-ttu-id="f6bbd-109">Não é possível criar um site com o mesmo URL de um site existente.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="f6bbd-110">Se eliminar um site e que desejem utilizar novamente o URL, é possível que o site eliminado continua a existir em **sites de eliminados**.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="f6bbd-111">Para gerir eliminar sites, consulte [Eliminar um Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="f6bbd-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="f6bbd-112">Para remover completamente um site com o Powershell, consulte o exemplo de cmdlet [Remover-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="f6bbd-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="f6bbd-113">Alguns utilizadores poderão não conseguir criar um site.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="f6bbd-114">Consulte [criação personalizada de sites gerir no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f6bbd-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="f6bbd-115">É possível que o site é apresentado-se a **Criar** mais do que o esperado.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="f6bbd-116">Se tiverem passado mais de 24 horas desde que a visualizou pela primeira vez a este problema, inicie uma permissão de suporte.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f6bbd-117">Em muitos casos, a Microsoft já estiver a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f6bbd-118">Forneça pelo menos 24 horas para concluir uma solução.</span><span class="sxs-lookup"><span data-stu-id="f6bbd-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="f6bbd-119">Se necessitar de criar um novo site de equipa que não inclui um grupo do Office 365,</span><span class="sxs-lookup"><span data-stu-id="f6bbd-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


