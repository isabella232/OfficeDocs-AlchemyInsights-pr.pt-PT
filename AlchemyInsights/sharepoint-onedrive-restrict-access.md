---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759091"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="befd0-102">Restringir o acesso no SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="befd0-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="befd0-103">Existem várias formas para restringir o acesso aos serviços do SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="befd0-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="befd0-104">Estes diversos métodos de restrição de acesso são descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="befd0-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="befd0-105">Restrição de permissão</span><span class="sxs-lookup"><span data-stu-id="befd0-105">Permission Restriction</span></span>

<span data-ttu-id="befd0-106">No SharePoint Online e OneDrive para a empresa, vamos restringir o acesso a itens como sites, ficheiros e pastas apenas concedendo acesso aos grupos/indivíduos que deveriam ter acesso.</span><span class="sxs-lookup"><span data-stu-id="befd0-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="befd0-107">Personalizar permissões para uma lista do SharePoint ou biblioteca</span><span class="sxs-lookup"><span data-stu-id="befd0-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="befd0-108">Personalizar permissões do site SharePoint</span><span class="sxs-lookup"><span data-stu-id="befd0-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="befd0-109">Alterar as permissões de uma subpasta</span><span class="sxs-lookup"><span data-stu-id="befd0-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="befd0-110">Controlar o acesso de dispositivos não geridos</span><span class="sxs-lookup"><span data-stu-id="befd0-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="befd0-111">Como um SharePoint ou administrador global no Office 365, pode bloquear ou limitar o acesso ao conteúdo SharePoint e OneDrive de dispositivos não geridos (esses híbrido AD associado ou compatível no Intune).</span><span class="sxs-lookup"><span data-stu-id="befd0-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="befd0-112">Restrição de localização de rede</span><span class="sxs-lookup"><span data-stu-id="befd0-112">Network Location Restriction</span></span>

<span data-ttu-id="befd0-113">Como um administrador de TI, pode controlar o acesso a recursos do SharePoint e OneDrive com base nas localizações de rede definido que considere fidedignos.</span><span class="sxs-lookup"><span data-stu-id="befd0-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="befd0-114">Isto também é conhecida como política baseada no local.</span><span class="sxs-lookup"><span data-stu-id="befd0-114">This is also known as location-based policy.</span></span> <span data-ttu-id="befd0-115">Para mais informações, consulte [controlar o acesso ao SharePoint Online e OneDrive dados com base na localização de rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="befd0-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="befd0-116">Restrição de bloqueio de sites</span><span class="sxs-lookup"><span data-stu-id="befd0-116">Site Lock Restriction</span></span> 

<span data-ttu-id="befd0-117">No SharePoint Online tem a capacidade para bloquear uma colecção de sites, para que ninguém tenha acesso.</span><span class="sxs-lookup"><span data-stu-id="befd0-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="befd0-118">Isto é definido através de PowerShell e a [Shell de gestão Online do SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizando a propriedade do [Conjunto-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.</span><span class="sxs-lookup"><span data-stu-id="befd0-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="befd0-119">Restringir os utilizadores criem sites ou subsites</span><span class="sxs-lookup"><span data-stu-id="befd0-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="befd0-120">Como um administrador do SharePoint ou administrador global do Office 365, pode permitir que os utilizadores criar e administrar os seus próprios sites SharePoint, determinar que tipo de sites podem criar e especifique a localização dos sites.</span><span class="sxs-lookup"><span data-stu-id="befd0-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="befd0-121">Para mais informações, consulte [Gerir a criação de sites no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="befd0-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

