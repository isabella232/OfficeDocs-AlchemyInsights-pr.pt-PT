---
title: Sincronização de perfil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554344"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="92eb5-102">Quando o meu perfil altera a sincronização para o aplicativo de perfil de usuário do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="92eb5-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="92eb5-103">O SharePoint Online usa o trabalho de timer de importação do Active Directory (importação do AD) para importar usuários e grupos para o aplicativo de perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="92eb5-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="92eb5-104">A importação de AD sincroniza alterações do repositório de diretórios do SharePoint Online para o aplicativo de perfil de usuário.</span><span class="sxs-lookup"><span data-stu-id="92eb5-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="92eb5-105">Essas alterações são processadas em lotes.</span><span class="sxs-lookup"><span data-stu-id="92eb5-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="92eb5-106">O trabalho de timer é executado até que as alterações sejam sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="92eb5-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="92eb5-107">O tempo que leva o trabalho a ser executado depende do número de alterações para processar.</span><span class="sxs-lookup"><span data-stu-id="92eb5-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="92eb5-108">Um grande número de alterações demora mais tempo.</span><span class="sxs-lookup"><span data-stu-id="92eb5-108">A large number of changes takes longer.</span></span> <span data-ttu-id="92eb5-109">O contrato de nível de serviço (SLA) informa que uma alteração para um usuário no diretório do SharePoint Online será refletida no aplicativo de perfil de usuário em 24 horas.</span><span class="sxs-lookup"><span data-stu-id="92eb5-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="92eb5-110">Mais informações sobre sincronização de perfil de usuário no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="92eb5-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

