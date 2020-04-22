---
title: Restringir o acesso no SharePoint ou oneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692776"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="16152-102">Restringir o acesso no SharePoint ou oneDrive</span><span class="sxs-lookup"><span data-stu-id="16152-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="16152-103">Existem muitas formas de restringir o acesso aos serviços SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="16152-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="16152-104">Estes vários métodos de restrição de acesso são descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="16152-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="16152-105">**Restrição de Permissão**</span><span class="sxs-lookup"><span data-stu-id="16152-105">**Permission Restriction**</span></span>

<span data-ttu-id="16152-106">No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, ficheiros e pastas, concedendo apenas acesso aos grupos/indivíduos que deveriam ter acesso.</span><span class="sxs-lookup"><span data-stu-id="16152-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="16152-107">Personalize permissões para uma lista de SharePoint ou biblioteca</span><span class="sxs-lookup"><span data-stu-id="16152-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="16152-108">Personalizar permissões do site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="16152-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="16152-109">Alterar as permissões numa subpasta</span><span class="sxs-lookup"><span data-stu-id="16152-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="16152-110">Controlar o acesso de dispositivos não geridos</span><span class="sxs-lookup"><span data-stu-id="16152-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="16152-111">Como um SharePoint ou administrador global, pode bloquear ou limitar o acesso ao conteúdo sharePoint e OneDrive a partir de dispositivos não geridos (aqueles que não são a D.C. híbridos unidos ou conformes no Intune).</span><span class="sxs-lookup"><span data-stu-id="16152-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="16152-112">**Restrição de Localização da Rede**</span><span class="sxs-lookup"><span data-stu-id="16152-112">**Network Location Restriction**</span></span>

<span data-ttu-id="16152-113">Como administrador de TI, pode controlar o acesso aos recursos SharePoint e OneDrive com base em localizações de rede definidas em que confia.</span><span class="sxs-lookup"><span data-stu-id="16152-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="16152-114">Isto também é conhecido como política baseada na localização.</span><span class="sxs-lookup"><span data-stu-id="16152-114">This is also known as location-based policy.</span></span> <span data-ttu-id="16152-115">Para mais informações, consulte [o acesso do Controlo aos dados SharePoint Online e OneDrive com base na localização da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="16152-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="16152-116">**Restrição de bloqueio do site**</span><span class="sxs-lookup"><span data-stu-id="16152-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="16152-117">Dentro do SharePoint Online tem a capacidade de bloquear uma coleção de site, para que ninguém tenha acesso.</span><span class="sxs-lookup"><span data-stu-id="16152-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="16152-118">Isto é definido através da PowerShell e da [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizando a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="16152-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="16152-119">**Restringir os utilizadores à criação de sites ou subsites**</span><span class="sxs-lookup"><span data-stu-id="16152-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="16152-120">Como administrador do SharePoint ou administrador global, pode permitir que os seus utilizadores criem e administram os seus próprios sites SharePoint, determinem que tipo de sites podem criar e especificar a localização dos sites.</span><span class="sxs-lookup"><span data-stu-id="16152-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="16152-121">Para mais informações, consulte Gerir a criação do [site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="16152-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

