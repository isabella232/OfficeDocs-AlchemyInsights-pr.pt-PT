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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320720"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando é que as alterações ao meu perfil são sincronizados com a Aplicação de Perfis de Utilizador do SharePoint?

O SharePoint Online utiliza a tarefa de temporador de Importação do Active Directory (Importação de AD) para importar utilizadores e grupos para a Aplicação de Perfis de Utilizador. 
  
1. AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. Estas alterações são processadas em lotes.
    
2. A tarefa de temporizador é executada até que as alterações sejam sincronizados.
    
**Nota:** O tempo que se demora a executar a tarefa depende do número de alterações a processar. Um grande número de alterações demora mais tempo. O Contrato de Nível de Serviço (SLA) indica que uma alteração a um utilizador no Diretório do SharePoint Online será refletida na Aplicação de Perfis de Utilizador no prazo de 24 horas. 
  
[Mais informações sobre a sincronização de perfis de utilizador no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

