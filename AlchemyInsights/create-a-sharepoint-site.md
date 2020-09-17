---
title: Criar um site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806950"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="1d4ad-102">Criar um site SharePoint</span><span class="sxs-lookup"><span data-stu-id="1d4ad-102">Create a SharePoint site</span></span>

<span data-ttu-id="1d4ad-103">Criar ou gerir sites a partir de [Sites Ativos](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) no Centro de Administração SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="1d4ad-104">Para obter mais informações, consulte [Gerir os sites no novo centro de administração do SharePoint.](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="1d4ad-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="1d4ad-105">Dicas:</span><span class="sxs-lookup"><span data-stu-id="1d4ad-105">Tips:</span></span>

- <span data-ttu-id="1d4ad-106">Não **é possível** criar um site com o mesmo URL de um site existente.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="1d4ad-107">Se apagou um site e deseja reutilizar o URL, é possível que o site eliminado ainda exista em [sites eliminados.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)</span><span class="sxs-lookup"><span data-stu-id="1d4ad-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="1d4ad-108">O site terá de ser permanentemente eliminado para reutilizar o URL.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="1d4ad-109">Para remover completamente um site com Powershell, consulte o exemplo [de cmdlet Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="1d4ad-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="1d4ad-110">Alguns utilizadores podem não ser capazes de criar um site.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="1d4ad-111">[Ver Gerir a criação do site no SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="1d4ad-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="1d4ad-112">É possível que o site apareça preso na **Criação** por mais tempo do que o esperado.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="1d4ad-113">Se passaram mais de 24 horas desde que viu este problema pela primeira vez, por favor, faça um bilhete de apoio.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1d4ad-114">Em muitos casos, já estamos a trabalhar numa solução.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1d4ad-115">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="1d4ad-115">Please give us at least 24 hours to complete a solution.</span></span>
