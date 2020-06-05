---
title: Partilhar com utilizadores externos não está a funcionar
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582786"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="575a4-102">Corrigir problemas de partilha de conteúdo do SharePoint com utilizadores externos</span><span class="sxs-lookup"><span data-stu-id="575a4-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="575a4-103">Certifique-se de que a partilha externa está ligada à sua organização:</span><span class="sxs-lookup"><span data-stu-id="575a4-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="575a4-104">Aceda à [ &amp; página de suplementos de serviços no centro de administração Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.</span><span class="sxs-lookup"><span data-stu-id="575a4-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="575a4-105">Certifique-se de que a definição está virada para "Ligado".</span><span class="sxs-lookup"><span data-stu-id="575a4-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="575a4-106">Se for selecionado "Apenas utilizadores externos existentes", certifique-se de que o utilizador externo está listado no centro de administração microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="575a4-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="575a4-107">Certifique-se de que a partilha externa foi ligada para o site.</span><span class="sxs-lookup"><span data-stu-id="575a4-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="575a4-108">Para uma coleção de site clássico:</span><span class="sxs-lookup"><span data-stu-id="575a4-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="575a4-109">No novo centro de administração do SharePoint, no painel esquerdo, clique nos **sites**.</span><span class="sxs-lookup"><span data-stu-id="575a4-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="575a4-110">Selecione o site ou sites, e na fita, clique em **Partilhar**.</span><span class="sxs-lookup"><span data-stu-id="575a4-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="575a4-111">Para um site de equipa que pertence a um grupo Microsoft 365, ou um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="575a4-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="575a4-112">Estes novos tipos de sites têm a mesma definição de partilha que a configuração da organização, a menos que a configuração em toda a organização permita partilhar ficheiros usando links que não requerem o acesso.</span><span class="sxs-lookup"><span data-stu-id="575a4-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="575a4-113">Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que se inscrevem.</span><span class="sxs-lookup"><span data-stu-id="575a4-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="575a4-114">Para alterar a definição para sites específicos, utilize o novo centro de administração sharePoint ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="575a4-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="575a4-115">[Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="575a4-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="575a4-116">A definição de partilha externa para qualquer site pode ser mais restritiva do que a configuração em toda a organização, mas não mais permissiva do que a configuração em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="575a4-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

