---
title: Site moderna, tal como o site de raiz
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057755"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="54ce9-102">Moderno site como site de raiz</span><span class="sxs-lookup"><span data-stu-id="54ce9-102">Modern site as root site</span></span>

<span data-ttu-id="54ce9-103">Os clientes de [Edição de destino](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) agora podem activar a experiência de site modernas de comunicação no site de raiz clássico de seu tenant do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="54ce9-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="54ce9-104">Esta funcionalidade pode ser activada ao executar um cmdlet PowerShell simple.</span><span class="sxs-lookup"><span data-stu-id="54ce9-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="54ce9-105">Sobre a execução com êxito do comando PowerShell, o site de raiz terá uma nova comunicação site home page.</span><span class="sxs-lookup"><span data-stu-id="54ce9-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="54ce9-106">Estão disponíveis no artigo [SPOCommSite activar](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)detalhes sobre os requisitos de cmdlet e funcionalidade do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="54ce9-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="54ce9-107">Vamos vai ser gradualmente graduais este problema, desligado por predefinição, para clientes alvo Release no início de Maio de 2019, e a expandir o estarão disponível em todo o mundo até ao final de Junho de 2019.</span><span class="sxs-lookup"><span data-stu-id="54ce9-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="54ce9-108">Continue a consultar o [Centro de mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) para outras funcionalidades novas com moderna.</span><span class="sxs-lookup"><span data-stu-id="54ce9-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="54ce9-109">**Importante**: não elimine o site de raiz clássico para criar um Site de comunicação modernos.</span><span class="sxs-lookup"><span data-stu-id="54ce9-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="54ce9-110">Não é suportada pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="54ce9-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="54ce9-111">Eliminar o site de raiz fará com que todos os sites SharePoint da sua organização inacessíveis a todos os utilizadores, até que restaure o site ou crie um novo site com o mesmo URL.</span><span class="sxs-lookup"><span data-stu-id="54ce9-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 