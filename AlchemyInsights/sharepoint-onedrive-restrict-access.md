---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053776"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f6ab6-102">Restringir o acesso no SharePoint ou no OneDrive</span><span class="sxs-lookup"><span data-stu-id="f6ab6-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f6ab6-103">Há muitas maneiras de restringir o acesso aos serviços SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f6ab6-104">Estes vários métodos de restrição de acesso são descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f6ab6-105">**Restrição de permissão**</span><span class="sxs-lookup"><span data-stu-id="f6ab6-105">**Permission Restriction**</span></span>

<span data-ttu-id="f6ab6-106">No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, arquivos e pastas, concedendo apenas acesso a esses grupos/indivíduos que devem ter acesso.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="f6ab6-107">Personalize as permissões para uma lista ou biblioteca do SharePoint</span><span class="sxs-lookup"><span data-stu-id="f6ab6-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="f6ab6-108">Personalize as permissões do site SharePoint</span><span class="sxs-lookup"><span data-stu-id="f6ab6-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="f6ab6-109">Alterar as permissões em uma subfoldera</span><span class="sxs-lookup"><span data-stu-id="f6ab6-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="f6ab6-110">Controlar o acesso de dispositivos não geridos</span><span class="sxs-lookup"><span data-stu-id="f6ab6-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f6ab6-111">Como um SharePoint ou administrador global no Office 365, você pode bloquear ou limitar o acesso ao conteúdo SharePoint e OneDrive de dispositivos não gerenciados (aqueles que não são AD híbridos se juntaram ou estiverem em conformidade em intune).</span><span class="sxs-lookup"><span data-stu-id="f6ab6-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f6ab6-112">**Restrição de localização da rede**</span><span class="sxs-lookup"><span data-stu-id="f6ab6-112">**Network Location Restriction**</span></span>

<span data-ttu-id="f6ab6-113">Como administrador de TI, você pode controlar o acesso aos recursos do SharePoint e do OneDrive com base em locais de rede definidos em que você confia.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f6ab6-114">Isso também é conhecido como política baseada em localização.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f6ab6-115">Para mais informações, consulte o [acesso ao Controle aos dados do SharePoint Online e do OneDrive com base na localização da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="f6ab6-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f6ab6-116">**Restrição de bloqueio do site**</span><span class="sxs-lookup"><span data-stu-id="f6ab6-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="f6ab6-117">Dentro sharepoint on-line você tem a capacidade de bloquear uma coleção do site, para que ninguém tenha acesso.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f6ab6-118">Isso é definido via PowerShell e o [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) usando a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f6ab6-119">**Restringir os usuários de criar sites ou subsites**</span><span class="sxs-lookup"><span data-stu-id="f6ab6-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="f6ab6-120">Como administrador do SharePoint ou administrador global do Office 365, você pode permitir que seus usuários criem e administrem seus próprios sites do SharePoint, determinar que tipo de sites eles podem criar e especificar a localização dos sites.</span><span class="sxs-lookup"><span data-stu-id="f6ab6-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f6ab6-121">Para mais informações, [consulte a criação do site gerenciar no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="f6ab6-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

