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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando é que o meu perfil muda de sincronização com a Aplicação de Perfil de Utilizador do SharePoint?

O SharePoint Online utiliza o temporizador de importação de diretório ativo (Importação aD) para importar utilizadores e grupos na Aplicação de Perfil de Utilizador. 
  
1. A AD Import sincroniza as alterações da Loja de Diretórios Online SharePoint para a Aplicação de Perfil do Utilizador. Estas alterações são processadas em lotes.
    
2. O trabalho do temporizador funciona até que as alterações sejam sincronizadas.
    
> [!NOTE]
> O tempo que o trabalho leva a funcionar depende do número de alterações ao processo. Um grande número de mudanças demora mais tempo. O Acordo de Nível de Serviço (SLA) estabelece que uma alteração a um utilizador no Diretório Online SharePoint será refletida na Aplicação de Perfil de Utilizador em 24 horas. 
  
[Mais informações sobre a sincronização do perfil do utilizador no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

