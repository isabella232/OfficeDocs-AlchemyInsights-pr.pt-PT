---
title: Partilhar com utilizadores externos não funciona
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
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747609"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e1b92-102">Corrigir problemas de partilha do conteúdo do SharePoint com utilizadores externos</span><span class="sxs-lookup"><span data-stu-id="e1b92-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e1b92-103">Certifique-se de partilha externa está activada para a sua organização:</span><span class="sxs-lookup"><span data-stu-id="e1b92-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e1b92-104">Vá para o [Serviços de &amp; página de suplementos no Centro de administração de Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)e clique em **Sites**.</span><span class="sxs-lookup"><span data-stu-id="e1b92-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e1b92-105">Certifique-se que a definição é ligada como "On".</span><span class="sxs-lookup"><span data-stu-id="e1b92-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="e1b92-106">Se estão seleccionados "Só utilizadores externos existentes", certifique-se o utilizador externo é listado no Centro de administração de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e1b92-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e1b92-107">Certifique-se externo partilha activada para o site.</span><span class="sxs-lookup"><span data-stu-id="e1b92-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="e1b92-108">Para uma colecção de sites clássico:</span><span class="sxs-lookup"><span data-stu-id="e1b92-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="e1b92-109">No novo Centro de administração do SharePoint, no painel da esquerda, clique em **sites**.</span><span class="sxs-lookup"><span data-stu-id="e1b92-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="e1b92-110">Seleccione o local ou locais e no Friso, clique em **partilhar**.</span><span class="sxs-lookup"><span data-stu-id="e1b92-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e1b92-111">Para um site de equipa que pertença a um grupo do Office 365 ou um site de comunicação:</span><span class="sxs-lookup"><span data-stu-id="e1b92-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e1b92-112">Estes novos tipos de site tem a mesma definição partilha como a definição de toda a organização, a menos que a definição de toda a organização permite a partilha de ficheiros a utilização de ligações que não requerem início de sessão.</span><span class="sxs-lookup"><span data-stu-id="e1b92-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="e1b92-113">Neste caso, os sites permitem a partilha com utilizadores externos novos e existentes que iniciar sessão.</span><span class="sxs-lookup"><span data-stu-id="e1b92-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="e1b92-114">Para alterar a definição para sites específicos, utilize o novo Centro de administração do SharePoint ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e1b92-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="e1b92-115">[Saiba mais](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="e1b92-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e1b92-116">A definição de partilha externa para qualquer site pode ser mais restritiva do que a definição de toda a organização, mas não mais permissivas podem permitir que a definição de toda a organização.</span><span class="sxs-lookup"><span data-stu-id="e1b92-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

