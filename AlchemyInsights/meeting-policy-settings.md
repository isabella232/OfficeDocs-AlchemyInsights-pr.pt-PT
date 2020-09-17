---
title: Definições de política de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794345"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerir políticas de reunião em Equipas da Microsoft

**Nota: Pode levar até 24 horas para que as alterações de política entrem em vigor para os utilizadores.** Pode não ser capaz de fazer alterações às políticas recém-criadas imediatamente; aguarde 4 horas e tente modificar uma política recém-criada novamente.

As políticas de reunião são usadas para controlar as funcionalidades disponíveis para reunir os participantes para reuniões que são agendadas pelos utilizadores da sua organização. Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipas (estas estão rotuladas "em breve" na documentação). Neste caso, ou se estiver a obter um erro como "Não podemos atualizar a política neste momento, mas tente novamente mais tarde" no centro de administração da Microsoft Teams, recomendamos que utilize o PowerShell para criar ou modificar as políticas de reunião de Equipas. 

Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:

- Para aprender a criar políticas, a fazer alterações e a atribuir os utilizadores à política, consulte [Gerir políticas de reunião em Equipas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para escoar alterações de política utilizando cmdlets PowerShell, consulte [a Visão Geral do PowerShell das Equipas](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [módulo Skype para Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) para equipas que cumprem políticas. 
    - Reveja a [documentação dos cmdlets da *-CSTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.

