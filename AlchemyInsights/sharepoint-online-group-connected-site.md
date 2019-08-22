---
title: Adicionar um grupo a um site do SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507858"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="d41b0-102">Problemas durante a criação ou de grupo ligado a sites SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d41b0-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="d41b0-103">Existem alguns problemas comuns encontrados quando criar ou recriar um grupo de ligado o site.</span><span class="sxs-lookup"><span data-stu-id="d41b0-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="d41b0-104">Se tiver eliminado um grupo e o respectivo site ligado e se pretende criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.</span><span class="sxs-lookup"><span data-stu-id="d41b0-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="d41b0-105">Transferir a [Shell de gestão de SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="d41b0-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="d41b0-106">Para obter mais informações acerca de como começar com o powershell, consulte [Introdução à Shell de gestão Online do SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="d41b0-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="d41b0-107">Remova o Site de Sites eliminada utilizando o cmdlet de powershell [Remover SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="d41b0-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="d41b0-108">Se estiver a criar um site ligado de grupo e receber um aviso de que outro grupo com o mesmo alias já existe, verifique os grupos existentes do [Office 365 partir do Centro de administração](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="d41b0-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="d41b0-109">Para resolver o problema, eliminar o grupo existente, se já não é necessário ou criar o site com um alias diferente atribuída.</span><span class="sxs-lookup"><span data-stu-id="d41b0-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="d41b0-110">Existem diferentes formas de criar e utilizar grupos modernos com o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d41b0-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="d41b0-111">Pode ligar a sites existentes a um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d41b0-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="d41b0-112">Para obter mais informações, consulte [ligar um grupo de Office 365 utilizando o ineterface de utilizador do SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="d41b0-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="d41b0-113">Para criar um site ligado de grupo do Office 365, terá de criar um Site de equipa.</span><span class="sxs-lookup"><span data-stu-id="d41b0-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="d41b0-114">Para obter mais informações, consulte [criar um site de equipa do SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="d41b0-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

