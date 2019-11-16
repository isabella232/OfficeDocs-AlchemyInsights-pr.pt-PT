---
title: Criar um site SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769602"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="9502d-102">Criar um site SharePoint</span><span class="sxs-lookup"><span data-stu-id="9502d-102">Create a SharePoint site</span></span>

<span data-ttu-id="9502d-103">Você pode ver o seguinte para obter informações sobre a criação do site SharePoint:</span><span class="sxs-lookup"><span data-stu-id="9502d-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="9502d-104">[Gerenciar sites no novo centro de administração do SharePoint:](https://docs.microsoft.com/sharepoint/manage-site-creation)saiba mais sobre as opções de criação do site, incluindo como criar um site clássico ou um site de equipes que não inclua um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9502d-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="9502d-105">[Crie um site de equipe no SharePoint:](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)saiba como criar um site de equipe.</span><span class="sxs-lookup"><span data-stu-id="9502d-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="9502d-106">Criar um site de [comunicação no SharePoint Online:](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)Saiba como criar um site de comunicações.</span><span class="sxs-lookup"><span data-stu-id="9502d-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="9502d-107">[Gerenciar sites no novo centro de administração sharepoint:](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)saiba como criar um site clássico ou um site de equipe que não inclua um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9502d-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="9502d-108">**Dicas:**</span><span class="sxs-lookup"><span data-stu-id="9502d-108">**Tips:**</span></span>
- <span data-ttu-id="9502d-109">Você não pode criar um site com a mesma URL de um site existente.</span><span class="sxs-lookup"><span data-stu-id="9502d-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="9502d-110">Se você excluiu um site e deseja reutilizar a URL, é possível que o site excluído ainda exista em **sites excluídos.**</span><span class="sxs-lookup"><span data-stu-id="9502d-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="9502d-111">Para gerenciar sites excluídos ver, [excluir um site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="9502d-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="9502d-112">Para remover completamente um site com powershell, consulte o exemplo de cmdlet [Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="9502d-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="9502d-113">Alguns usuários podem não ser capazes de criar um site.</span><span class="sxs-lookup"><span data-stu-id="9502d-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="9502d-114">Veja [gerenciar a criação do site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="9502d-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="9502d-115">É possível que o site parece preso em **criar** mais tempo do que o esperado.</span><span class="sxs-lookup"><span data-stu-id="9502d-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="9502d-116">Se mais de 24 horas se passaram desde que você viu pela primeira vez este problema, por favor, registre um bilhete de suporte.</span><span class="sxs-lookup"><span data-stu-id="9502d-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9502d-117">Em muitos casos, já estamos trabalhando em uma solução.</span><span class="sxs-lookup"><span data-stu-id="9502d-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9502d-118">Por favor, dê-nos pelo menos 24 horas para completar uma solução.</span><span class="sxs-lookup"><span data-stu-id="9502d-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="9502d-119">Se você precisa criar um novo site de equipe que não inclua um grupo do Office 365,</span><span class="sxs-lookup"><span data-stu-id="9502d-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


