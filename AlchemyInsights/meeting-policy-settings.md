---
title: Definições de políticas de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627585"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerenciar políticas de reunião em equipes da Microsoft

As políticas de reunião são usadas para controlar os recursos disponíveis para atender os participantes para reuniões agendadas pelos usuários em sua organização. Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipes (elas são rotuladas como "em breve" na documentação). Neste caso, ou se você está recebendo um erro como "Não podemos atualizar a política agora, mas experimentá-lo novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as políticas de reunião das equipes. 

Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre a criação de políticas, fazer mudanças e atribuir os usuários à política, [consulte as políticas de reunião em equipes.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Para fazer alterações de política usando cmdlets PowerShell, consulte [equipes PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [módulo Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) para políticas de reunião de equipes. 
    - Analise a [documentação de cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.

**Nota:** Pode levar até 24 horas para que as alterações de política entrem em vigor para os usuários. Você pode não ser capaz de fazer alterações nas políticas recém-criadas imediatamente; espere 4 horas e tente modificar uma política recém-criada novamente. Se você ainda está tendo problemas, tente PowerShell.  