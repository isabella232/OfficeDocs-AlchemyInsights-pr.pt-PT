---
title: Dar aos utilizadores acesso ao SharePoint e ao OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721815"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="7c8e3-102">Dar aos utilizadores acesso ao SharePoint e ao OneDrive</span><span class="sxs-lookup"><span data-stu-id="7c8e3-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="7c8e3-103">Se um site oneDrive ou SharePoint não estiver disponível para vários utilizadores que anteriormente tiveram acesso, pode haver um problema de serviço temporário.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="7c8e3-104">Verifique o painel de saúde de serviço</span><span class="sxs-lookup"><span data-stu-id="7c8e3-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="7c8e3-105">Se quiser que as pessoas da sua organização possam iniciar sessão e utilizar o SharePoint e o OneDrive, tem de adicionar contas para elas e certificar-se de que têm uma licença que lhes dá acesso ao SharePoint e ao OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="7c8e3-106">A forma mais fácil de adicionar utilizadores é no centro de administração da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="7c8e3-107">Vá para a página de [utilizadores Ativos no centro de administração da Microsoft 365,](https://portal.office.com/adminportal/home#/users)e depois clique em Adicionar um **utilizador**.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="7c8e3-108">Preencha as informações para o utilizador e certifique-se de que, sob **licençado Produto,** é atribuída uma licença e o **SharePoint Online** é selecionado.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="7c8e3-109">Note que se permitir a partilha externa na sua organização, os utilizadores podem partilhar o sharePoint e o conteúdo OneDrive com pessoas fora da organização.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="7c8e3-110">Não precisa de dar licenças a estes utilizadores externos.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="7c8e3-111">Também não precisa de adicionar contas para elas, a menos que a partilha seja definida para "Apenas utilizadores externos existentes".</span><span class="sxs-lookup"><span data-stu-id="7c8e3-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="7c8e3-112">Nesse caso, se as pessoas não estiverem no diretório da sua organização, precisa adicioná-las como utilizadores convidados no centro de administração da AD Azure.</span><span class="sxs-lookup"><span data-stu-id="7c8e3-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

