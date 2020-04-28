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
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913013"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="2bee6-102">Corrigir problemas de partilha de conteúdo do SharePoint com utilizadores externos</span><span class="sxs-lookup"><span data-stu-id="2bee6-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="2bee6-103">Certifique-se de que a partilha externa está ligada para a sua organização:</span><span class="sxs-lookup"><span data-stu-id="2bee6-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="2bee6-104">Vá à página de [add-ins dos Serviços &amp; no centro de administração da Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), e clique em **Sites**.</span><span class="sxs-lookup"><span data-stu-id="2bee6-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="2bee6-105">Certifique-se de que a definição está virada para "On".</span><span class="sxs-lookup"><span data-stu-id="2bee6-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="2bee6-106">Se "Apenas forem selecionados utilizadores externos existentes", certifique-se de que o utilizador externo está listado no centro de administração da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2bee6-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="2bee6-107">Certifique-se de que a partilha externa foi ligada para o site.</span><span class="sxs-lookup"><span data-stu-id="2bee6-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="2bee6-108">Para uma coleção clássica do site:</span><span class="sxs-lookup"><span data-stu-id="2bee6-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="2bee6-109">No novo centro de administração do SharePoint, no painel esquerdo, clique **em sites**.</span><span class="sxs-lookup"><span data-stu-id="2bee6-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="2bee6-110">Selecione o site ou os sites e na fita, clique em **Partilhar**.</span><span class="sxs-lookup"><span data-stu-id="2bee6-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="2bee6-111">Para um site de equipa que pertence a um grupo Microsoft 365, ou a um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="2bee6-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="2bee6-112">Estes novos tipos de sites têm a mesma definição de partilha que a sua configuração em toda a organização, a menos que a definição em toda a organização permita a partilha de ficheiros usando links que não requerem iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="2bee6-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="2bee6-113">Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que se inscrevam.</span><span class="sxs-lookup"><span data-stu-id="2bee6-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="2bee6-114">Para alterar a definição para sites específicos, utilize o novo centro de administração do SharePoint ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2bee6-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="2bee6-115">[Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="2bee6-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="2bee6-116">O cenário de partilha externa para qualquer site pode ser mais restritivo do que o ambiente em toda a organização, mas não mais permissivo do que o ambiente em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="2bee6-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

