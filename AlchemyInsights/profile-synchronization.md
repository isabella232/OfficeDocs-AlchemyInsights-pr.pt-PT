---
title: Sincronização de perfil
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768124"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="25e20-102">Quando é que o meu perfil muda de sincronização com a Aplicação de Perfil de Utilizador do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="25e20-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="25e20-103">O SharePoint Online utiliza o temporizador de importação de diretório ativo (Importação aD) para importar utilizadores e grupos na Aplicação de Perfil de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="25e20-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="25e20-104">A AD Import sincroniza as alterações da Loja de Diretórios Online SharePoint para a Aplicação de Perfil do Utilizador.</span><span class="sxs-lookup"><span data-stu-id="25e20-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="25e20-105">Estas alterações são processadas em lotes.</span><span class="sxs-lookup"><span data-stu-id="25e20-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="25e20-106">O trabalho do temporizador funciona até que as alterações sejam sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="25e20-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="25e20-107">O tempo que o trabalho leva a funcionar depende do número de alterações ao processo.</span><span class="sxs-lookup"><span data-stu-id="25e20-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="25e20-108">Um grande número de mudanças demora mais tempo.</span><span class="sxs-lookup"><span data-stu-id="25e20-108">A large number of changes takes longer.</span></span> <span data-ttu-id="25e20-109">O Acordo de Nível de Serviço (SLA) estabelece que uma alteração a um utilizador no Diretório Online SharePoint será refletida na Aplicação de Perfil de Utilizador em 24 horas.</span><span class="sxs-lookup"><span data-stu-id="25e20-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="25e20-110">Mais informações sobre a sincronização do perfil do utilizador no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="25e20-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

