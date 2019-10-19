---
title: Compartilhar com usuários externos não está funcionando
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502242"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="b09fd-102">Corrigir problemas de compartilhamento de conteúdo do SharePoint com usuários externos</span><span class="sxs-lookup"><span data-stu-id="b09fd-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="b09fd-103">Certifique-se de que o compartilhamento externo esteja ativado para sua organização:</span><span class="sxs-lookup"><span data-stu-id="b09fd-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="b09fd-104">Vá para a [página &amp; de suplementos de serviços no centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **sites**.</span><span class="sxs-lookup"><span data-stu-id="b09fd-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="b09fd-105">Certifique-se de que a definição está virada para "ligado".</span><span class="sxs-lookup"><span data-stu-id="b09fd-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="b09fd-106">Se "somente usuários externos existentes" estiver selecionado, certifique-se de que o usuário externo está listado no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b09fd-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="b09fd-107">Certifique-se de que o compartilhamento externo esteja ativado para o site.</span><span class="sxs-lookup"><span data-stu-id="b09fd-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="b09fd-108">Para um conjunto de sites clássico:</span><span class="sxs-lookup"><span data-stu-id="b09fd-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="b09fd-109">No novo centro de administração do SharePoint, no painel esquerdo, clique em **sites**.</span><span class="sxs-lookup"><span data-stu-id="b09fd-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="b09fd-110">Selecione o site ou sites e, na faixa de opções, clique em **compartilhamento**.</span><span class="sxs-lookup"><span data-stu-id="b09fd-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="b09fd-111">Para um site de equipe que pertence a um grupo do Office 365 ou um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="b09fd-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="b09fd-112">Esses novos tipos de site têm a mesma configuração de compartilhamento que a configuração de toda a organização, a menos que a configuração de toda a organização permita o compartilhamento de arquivos usando links que não exijam login.</span><span class="sxs-lookup"><span data-stu-id="b09fd-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="b09fd-113">Nesse caso, os sites permitem o compartilhamento com usuários externos novos e existentes que fizerem login.</span><span class="sxs-lookup"><span data-stu-id="b09fd-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="b09fd-114">Para alterar a configuração de sites específicos, use o novo centro de administração do SharePoint ou o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b09fd-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="b09fd-115">[Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="b09fd-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="b09fd-116">A configuração de compartilhamento externo para qualquer site pode ser mais restritiva do que a configuração de toda a organização, mas não mais permissiva do que a configuração de toda a organização.</span><span class="sxs-lookup"><span data-stu-id="b09fd-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

