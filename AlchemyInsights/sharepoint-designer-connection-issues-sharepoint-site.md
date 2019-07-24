---
title: Problemas de ligação do SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840562"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="98e85-102">Problemas de ligação do SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="98e85-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="98e85-103">Se o SharePoint Designer está com problemas de ligação aos SharePoint sites, tente as seguintes soluções comuns.</span><span class="sxs-lookup"><span data-stu-id="98e85-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="98e85-104">Passo 1: Verificar se o SharePoint Designer 2013 é actualizado com o [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e [2 de Agosto de 2016 actualização para o SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="98e85-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="98e85-105">Passo 2: Limpe os ficheiros de local cache:</span><span class="sxs-lookup"><span data-stu-id="98e85-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="98e85-106">Feche o SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="98e85-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="98e85-107">No computador local, remova todos os ficheiros localizados em cada uma das seguintes pastas.</span><span class="sxs-lookup"><span data-stu-id="98e85-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="98e85-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="98e85-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="98e85-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="98e85-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="98e85-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="98e85-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="98e85-111">Abra o SharePoint Designer 2013 e introduza a conta novamente para verificar se funciona.</span><span class="sxs-lookup"><span data-stu-id="98e85-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="98e85-112">Passo 3: [Activar a autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="98e85-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="98e85-113">Passo 4: Os administradores serão necessário **Permitir Script personalizado** nas definições do Centro de administração do SharePoint para permitir a ligação do SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="98e85-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="98e85-114">Consulte [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="98e85-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


