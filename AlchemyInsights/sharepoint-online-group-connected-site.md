---
title: Adicione um grupo a um site do SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771219"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="c4968-102">Problemas ao criar um site conectado a grupo no SharePoint</span><span class="sxs-lookup"><span data-stu-id="c4968-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="c4968-103">Algumas questões comuns encontradas ao criar ou recriar um site conectado a grupo.</span><span class="sxs-lookup"><span data-stu-id="c4968-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="c4968-104">Se eliminou um grupo e o seu site conectado e deseja criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.</span><span class="sxs-lookup"><span data-stu-id="c4968-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="c4968-105">Baixar [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="c4968-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="c4968-106">Para obter mais informações sobre como começar com a Powershell, consulte [Começar com a SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)</span><span class="sxs-lookup"><span data-stu-id="c4968-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="c4968-107">Remova o Site de Sites eliminados utilizando o [cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="c4968-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="c4968-108">A Powershell é necessária para eliminar permanentemente os sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="c4968-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="c4968-109">Se estiver a criar um site ligado ao grupo e receber um aviso: Outro grupo com o mesmo pseudónimo já existe , verifique os **grupos**existentes do [centro de administração Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="c4968-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="c4968-110">Para resolver o problema, elimine o grupo existente se já não for necessário ou crie o site com um pseudónimo diferente atribuído.</span><span class="sxs-lookup"><span data-stu-id="c4968-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="c4968-111">Existem diferentes formas de criar e usar grupos modernos com o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c4968-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="c4968-112">Pode ligar os sites existentes a um grupo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4968-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="c4968-113">Para obter mais informações, consulte [Conecte um grupo Microsoft 365 utilizando a interface de utilizador do SharePoint.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="c4968-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="c4968-114">Para criar um site ligado ao grupo Microsoft 365, terá de criar um [Site de Equipa](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="c4968-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
