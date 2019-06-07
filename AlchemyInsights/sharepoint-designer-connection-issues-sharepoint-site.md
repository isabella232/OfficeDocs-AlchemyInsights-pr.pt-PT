---
title: Níveis de permissão SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760703"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="a9774-102">Problemas de ligação do SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="a9774-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="a9774-103">Se o SharePoint Designer está com problemas de ligação aos SharePoint sites, tente as seguintes soluções comuns.</span><span class="sxs-lookup"><span data-stu-id="a9774-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="a9774-104">Passo 1: Verificar se o SharePoint Designer é actualizado.</span><span class="sxs-lookup"><span data-stu-id="a9774-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="a9774-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="a9774-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="a9774-106">O SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="a9774-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="a9774-107">Actualização para o SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="a9774-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="a9774-108">Passo 2: Limpar os ficheiros de local cache</span><span class="sxs-lookup"><span data-stu-id="a9774-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="a9774-109">Feche o SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a9774-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="a9774-110">No computador local, procure as seguintes pastas para remover ficheiros em cache.</span><span class="sxs-lookup"><span data-stu-id="a9774-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="a9774-111">Clique em Iniciar, executar e eliminar todos os ficheiros encontrados em cada um a seguir localizações.</span><span class="sxs-lookup"><span data-stu-id="a9774-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="a9774-112">Servidor de %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="a9774-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="a9774-113">Abra o SharePoint Designer 2013 e introduza a conta novamente para verificar se funciona.</span><span class="sxs-lookup"><span data-stu-id="a9774-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="a9774-114">Passo 3: [Activar a autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a9774-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="a9774-115">Passo 4: Os administradores serão necessário permitir Script personalizado para permitir a ligação do SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="a9774-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="a9774-116">Para obter passos detalhados, exemplos e considerações consulte [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="a9774-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


