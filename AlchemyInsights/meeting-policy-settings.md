---
title: Definições de política de reunião
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825454"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerir políticas de reunião em Equipas da Microsoft

**Nota: Pode levar até 24 horas para que as alterações de política entrem em vigor para os utilizadores.** Pode não ser capaz de fazer alterações às políticas recém-criadas imediatamente; aguarde 4 horas e tente modificar uma política recém-criada novamente.

As políticas de reunião são usadas para controlar as funcionalidades disponíveis para reunir os participantes para reuniões que são agendadas pelos utilizadores da sua organização. Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipas (estas estão rotuladas "em breve" na documentação). Neste caso, ou se estiver a obter um erro como "Não podemos atualizar a política neste momento, mas tente novamente mais tarde" no centro de administração da Microsoft Teams, recomendamos que utilize o PowerShell para criar ou modificar as políticas de reunião de Equipas. 

Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:

- Para aprender a criar políticas, a fazer alterações e a atribuir os utilizadores à política, consulte [Gerir políticas de reunião em Equipas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para escoar alterações de política utilizando cmdlets PowerShell, consulte [a Visão Geral do PowerShell das Equipas](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [módulo Skype para Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) para equipas que cumprem políticas. 
    - Reveja a [documentação dos cmdlets da *-CSTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.

