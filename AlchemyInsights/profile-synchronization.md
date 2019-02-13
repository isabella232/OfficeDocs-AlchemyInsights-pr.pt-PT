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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920099"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando as alterações de perfil sincronizar a aplicação de perfil de utilizador do SharePoint?

SharePoint Online utiliza a tarefa de temporizador de importação Active Directory (AD importar) para importar utilizadores e grupos para a aplicação do perfil de utilizador. 
  
1. Importação de AD sincroniza as alterações do arquivo de directório Online do SharePoint para a aplicação do perfil de utilizador. Estas alterações são processadas em lotes.
    
2. A tarefa de temporizador é executada até que as alterações estarem sincronizadas.
    
> [!NOTE]
> O tempo que demora a tarefa para ser executada depende do número de alterações para processar. Um grande número de alterações é mais demorado. O acordo de nível de serviço (SLA) indica que uma alteração a um utilizador no directório Online SharePoint será reflectida na aplicação de perfil de utilizador nas 24 horas. 
  
[Obter mais informações sobre a sincronização de perfis de utilizador no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

