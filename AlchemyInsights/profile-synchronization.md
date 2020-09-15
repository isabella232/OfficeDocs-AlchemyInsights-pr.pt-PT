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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando é que o meu perfil muda de sincronização para a Aplicação de Perfil de Utilizador SharePoint?

O SharePoint Online utiliza o trabalho de timer de importação de diretório ativo (Importação AD) para importar utilizadores e grupos para a Aplicação de Perfil do Utilizador. 
  
1. A AD Import sincroniza as alterações da Loja de Diretório Online SharePoint para a Aplicação de Perfil do Utilizador. Estas alterações são processadas em lotes.
    
2. O trabalho do temporizador funciona até que as alterações sejam sincronizadas.
    
> [!NOTE]
> O tempo que o trabalho leva para correr depende do número de alterações ao processo. Um grande número de mudanças demora mais tempo. O Acordo de Nível de Serviço (SLA) afirma que uma alteração para um utilizador no Diretório Online SharePoint será refletida na Aplicação de Perfil do Utilizador em 24 horas. 
  
[Mais informações sobre a sincronização do perfil do utilizador no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

