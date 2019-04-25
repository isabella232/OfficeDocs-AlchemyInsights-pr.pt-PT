---
title: Sincronização de perfis
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371995"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="f0738-102">Quando as alterações de perfil sincronizar a aplicação de perfil de utilizador do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="f0738-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="f0738-103">SharePoint Online utiliza a tarefa de temporizador de importação Active Directory (AD importar) para importar utilizadores e grupos para a aplicação do perfil de utilizador.</span><span class="sxs-lookup"><span data-stu-id="f0738-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="f0738-104">Importação de AD sincroniza as alterações do arquivo de directório Online do SharePoint para a aplicação do perfil de utilizador.</span><span class="sxs-lookup"><span data-stu-id="f0738-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="f0738-105">Estas alterações são processadas em lotes.</span><span class="sxs-lookup"><span data-stu-id="f0738-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="f0738-106">A tarefa de temporizador é executada até que as alterações estarem sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="f0738-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="f0738-107">O tempo que demora a tarefa para ser executada depende do número de alterações para processar.</span><span class="sxs-lookup"><span data-stu-id="f0738-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="f0738-108">Um grande número de alterações é mais demorado.</span><span class="sxs-lookup"><span data-stu-id="f0738-108">A large number of changes takes longer.</span></span> <span data-ttu-id="f0738-109">O acordo de nível de serviço (SLA) indica que uma alteração a um utilizador no directório Online SharePoint será reflectida na aplicação de perfil de utilizador nas 24 horas.</span><span class="sxs-lookup"><span data-stu-id="f0738-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="f0738-110">Obter mais informações sobre a sincronização de perfis de utilizador no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f0738-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

