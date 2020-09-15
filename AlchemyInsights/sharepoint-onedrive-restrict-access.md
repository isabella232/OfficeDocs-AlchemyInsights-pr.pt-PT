---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700466"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="fcedf-102">Restringir o acesso no SharePoint ou no OneDrive</span><span class="sxs-lookup"><span data-stu-id="fcedf-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="fcedf-103">Existem muitas formas de restringir o acesso aos serviços SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fcedf-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="fcedf-104">Estes vários métodos de restrição de acesso são descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="fcedf-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="fcedf-105">**Restrição de Permissão**</span><span class="sxs-lookup"><span data-stu-id="fcedf-105">**Permission Restriction**</span></span>

<span data-ttu-id="fcedf-106">No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, ficheiros e pastas, concedendo apenas acesso a esses grupos/indivíduos que deveriam ter acesso.</span><span class="sxs-lookup"><span data-stu-id="fcedf-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="fcedf-107">Personalize permissões para uma lista ou biblioteca sharePoint</span><span class="sxs-lookup"><span data-stu-id="fcedf-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="fcedf-108">Personalize permissões do site SharePoint</span><span class="sxs-lookup"><span data-stu-id="fcedf-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="fcedf-109">Altere as permissões numa sub-dobra</span><span class="sxs-lookup"><span data-stu-id="fcedf-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="fcedf-110">Controlar o acesso de dispositivos não geridos</span><span class="sxs-lookup"><span data-stu-id="fcedf-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="fcedf-111">Como administrador do SharePoint ou global, pode bloquear ou limitar o acesso ao conteúdo sharePoint e OneDrive a partir de dispositivos não geridos (aqueles que não são híbridos ad joined ou compliant in Intune).</span><span class="sxs-lookup"><span data-stu-id="fcedf-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="fcedf-112">**Restrição de localização da rede**</span><span class="sxs-lookup"><span data-stu-id="fcedf-112">**Network Location Restriction**</span></span>

<span data-ttu-id="fcedf-113">Como administrador de TI, pode controlar o acesso aos recursos sharePoint e OneDrive com base em localizações de rede definidas em que confia.</span><span class="sxs-lookup"><span data-stu-id="fcedf-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="fcedf-114">Isto também é conhecido como política baseada na localização.</span><span class="sxs-lookup"><span data-stu-id="fcedf-114">This is also known as location-based policy.</span></span> <span data-ttu-id="fcedf-115">Para mais informações, consulte [o acesso ao Control para os dados do SharePoint Online e do OneDrive com base na localização da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="fcedf-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="fcedf-116">**Restrição de bloqueio do site**</span><span class="sxs-lookup"><span data-stu-id="fcedf-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="fcedf-117">No SharePoint Online tem a capacidade de bloquear uma coleção de sites, para que ninguém tenha acesso.</span><span class="sxs-lookup"><span data-stu-id="fcedf-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="fcedf-118">Isto é definido através do PowerShell e da [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizando a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="fcedf-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="fcedf-119">**Restringir os utilizadores da criação de sites ou subsites**</span><span class="sxs-lookup"><span data-stu-id="fcedf-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="fcedf-120">Como administrador do SharePoint ou administrador global, pode permitir que os seus utilizadores criem e administram os seus próprios sites SharePoint, determinem que tipo de sites podem criar e especificar a localização dos sites.</span><span class="sxs-lookup"><span data-stu-id="fcedf-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="fcedf-121">Para mais informações, consulte [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="fcedf-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

