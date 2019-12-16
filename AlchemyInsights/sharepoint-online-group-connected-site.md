---
title: Adicionar um grupo a um site do SharePoint
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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051112"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="c58d2-102">Problemas ao criar ou agrupar sites conectados no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c58d2-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="c58d2-103">Há um par de problemas comuns encontrados ao criar ou recriar um site conectado em grupo.</span><span class="sxs-lookup"><span data-stu-id="c58d2-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="c58d2-104">Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, você precisará remover permanentemente o site anterior.</span><span class="sxs-lookup"><span data-stu-id="c58d2-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="c58d2-105">Baixe [o Shell de gestão SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="c58d2-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="c58d2-106">Para mais informações sobre como começar com powershell, veja [começar com sharepoint online management shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="c58d2-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="c58d2-107">Retire o site de sites excluídos usando o cmdlet de casca de potência [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="c58d2-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="c58d2-108">Se você está criando um site conectado em grupo e receber um aviso Outro grupo com o mesmo pseudônimo já existe, verifique os grupos existentes do [Office 365 do Centro de Administração.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)</span><span class="sxs-lookup"><span data-stu-id="c58d2-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="c58d2-109">Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou criar o site com um pseudônimo diferente atribuído.</span><span class="sxs-lookup"><span data-stu-id="c58d2-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="c58d2-110">Existem diferentes maneiras de criar e usar grupos modernos com sharepoint.</span><span class="sxs-lookup"><span data-stu-id="c58d2-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="c58d2-111">Você pode conectar sites existentes a um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="c58d2-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="c58d2-112">Para mais informações, [consulte o grupo Connect an Office 365 usando o ineterface do usuário Do SharePoint.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)</span><span class="sxs-lookup"><span data-stu-id="c58d2-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="c58d2-113">Para criar um site conectado ao grupo Office 365, você precisará criar um site de equipe.</span><span class="sxs-lookup"><span data-stu-id="c58d2-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="c58d2-114">Para mais informações, consulte criar um site de [equipe no SharePoint.](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)</span><span class="sxs-lookup"><span data-stu-id="c58d2-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

