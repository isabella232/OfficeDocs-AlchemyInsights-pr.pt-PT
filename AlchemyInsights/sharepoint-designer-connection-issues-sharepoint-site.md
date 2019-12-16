---
title: Problemas de conexão sharepoint designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051724"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="6151a-102">Problemas de conexão sharepoint designer</span><span class="sxs-lookup"><span data-stu-id="6151a-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="6151a-103">Se o SharePoint Designer está enfrentando problemas de conexão com sites do SharePoint, tente as seguintes soluções comuns.</span><span class="sxs-lookup"><span data-stu-id="6151a-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="6151a-104">Etapa 1: Verifique se o SharePoint Designer 2013 é atualizado com o Pacote de Serviço de [Designer SharePoint 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e a atualização de 2 de agosto de [2016 para designer sharepoint 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="6151a-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="6151a-105">Passo 2: Limpe os arquivos de cache locais:</span><span class="sxs-lookup"><span data-stu-id="6151a-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="6151a-106">Fechar SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="6151a-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="6151a-107">No computador local, remova todos os arquivos encontrados em cada uma das seguintes pastas.</span><span class="sxs-lookup"><span data-stu-id="6151a-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="6151a-108">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\Web Server Extensões \Cache</span><span class="sxs-lookup"><span data-stu-id="6151a-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="6151a-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="6151a-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="6151a-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="6151a-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="6151a-111">Abra sharepoint designer 2013 e digite a conta novamente para ver se ele funciona.</span><span class="sxs-lookup"><span data-stu-id="6151a-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="6151a-112">Etapa 3: [Habilite autenticação moderna para o Office 2013 em dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6151a-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="6151a-113">Passo 4: Os administradores precisarão **permitir o script personalizado** nas configurações do SharePoint Admin Center para permitir a conexão SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="6151a-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="6151a-114">Veja [permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="6151a-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


