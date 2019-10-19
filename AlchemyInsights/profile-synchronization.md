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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando o meu perfil altera a sincronização para o aplicativo de perfil de usuário do SharePoint?

O SharePoint Online usa o trabalho de timer de importação do Active Directory (importação do AD) para importar usuários e grupos para o aplicativo de perfil de usuário. 
  
1. A importação de AD sincroniza alterações do repositório de diretórios do SharePoint Online para o aplicativo de perfil de usuário. Essas alterações são processadas em lotes.
    
2. O trabalho de timer é executado até que as alterações sejam sincronizadas.
    
> [!NOTE]
> O tempo que leva o trabalho a ser executado depende do número de alterações para processar. Um grande número de alterações demora mais tempo. O contrato de nível de serviço (SLA) informa que uma alteração para um usuário no diretório do SharePoint Online será refletida no aplicativo de perfil de usuário em 24 horas. 
  
[Mais informações sobre sincronização de perfil de usuário no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

