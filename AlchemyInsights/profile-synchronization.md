---
title: Sincronização de perfis
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801780"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="ecfe3-102">Quando é que o meu perfil muda de sincronização para a Aplicação de Perfil de Utilizador SharePoint?</span><span class="sxs-lookup"><span data-stu-id="ecfe3-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="ecfe3-103">O SharePoint Online utiliza o trabalho de timer de importação de diretório ativo (Importação AD) para importar utilizadores e grupos para a Aplicação de Perfil do Utilizador.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="ecfe3-104">A AD Import sincroniza as alterações da Loja de Diretório Online SharePoint para a Aplicação de Perfil do Utilizador.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="ecfe3-105">Estas alterações são processadas em lotes.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="ecfe3-106">O trabalho do temporizador funciona até que as alterações sejam sincronizadas.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="ecfe3-107">O tempo que o trabalho leva para correr depende do número de alterações ao processo.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="ecfe3-108">Um grande número de mudanças demora mais tempo.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-108">A large number of changes takes longer.</span></span> <span data-ttu-id="ecfe3-109">O Acordo de Nível de Serviço (SLA) afirma que uma alteração para um utilizador no Diretório Online SharePoint será refletida na Aplicação de Perfil do Utilizador em 24 horas.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="ecfe3-110">Mais informações sobre a sincronização do perfil do utilizador no SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ecfe3-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

