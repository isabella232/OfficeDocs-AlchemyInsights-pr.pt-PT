---
title: Adicione um grupo a um site do SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642155"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="1509e-102">Problemas ao criar um site ligado ao grupo no SharePoint</span><span class="sxs-lookup"><span data-stu-id="1509e-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="1509e-103">Algumas questões comuns encontraram-se ao criar ou recriar um site ligado ao grupo.</span><span class="sxs-lookup"><span data-stu-id="1509e-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="1509e-104">Se tiver eliminado um grupo e o seu site conectado e pretender criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.</span><span class="sxs-lookup"><span data-stu-id="1509e-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="1509e-105">Baixar [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="1509e-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="1509e-106">Para mais informações sobre começar com a Powershell, consulte [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="1509e-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="1509e-107">Remova o Site dos Sites Eliminados utilizando o cmdlet [remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="1509e-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="1509e-108">A Powershell é necessária para eliminar permanentemente os sites do grupo.</span><span class="sxs-lookup"><span data-stu-id="1509e-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="1509e-109">Se estiver a criar um site ligado ao grupo e receber um aviso: **Outro grupo com o mesmo pseudónimo já existe,** verifique os grupos existentes do Microsoft [365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="1509e-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="1509e-110">Para resolver o problema, elimine o grupo existente se já não for necessário ou criar o site com um pseudónimo diferente atribuído.</span><span class="sxs-lookup"><span data-stu-id="1509e-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="1509e-111">Existem diferentes formas de criar e usar grupos modernos com o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1509e-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="1509e-112">Pode ligar os sites existentes a um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1509e-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="1509e-113">Para mais informações, consulte [Connect um grupo Office 365 utilizando a interface de utilizador do SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="1509e-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="1509e-114">Para criar um site ligado ao grupo Office 365, terá de criar um Site de [Equipa.](https://admin.microsoft.com/sharepoint)</span><span class="sxs-lookup"><span data-stu-id="1509e-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
