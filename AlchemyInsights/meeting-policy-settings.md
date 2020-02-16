---
title: Definições políticas de reunião
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042855"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerir as políticas de reunião em Equipas microsoft

**Nota: Pode levar até 24 horas para que as alterações de política entrem em vigor para os utilizadores.** Pode não ser capaz de fazer alterações às políticas recém-criadas imediatamente; esperar 4 horas e tentar modificar uma política recém-criada novamente.

As políticas de reunião são usadas para controlar as funcionalidades que estão disponíveis para reunir os participantes para reuniões agendadas pelos utilizadores da sua organização. Algumas características das políticas de reunião podem ainda não ser implementadas no centro de administração das Equipas (estas estão rotuladas como "em breve" na documentação). Neste caso, ou se estiver a ter um erro como "Não podemos atualizar a apólice agora, mas tente novamente mais tarde" no centro de administração da Microsoft Teams, recomendamos que use o PowerShell para criar ou modificar as políticas de reunião das Equipas. 

Para obter mais informações sobre as políticas de reunião, consulte os seguintes recursos:

- Para aprender sobre a criação de políticas, fazer alterações e atribuir utilizadores à política, consulte [gerir as políticas de reunião em Equipas.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Para fazer alterações de política utilizando cmdlets PowerShell, consulte a visão geral do [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [módulo Skype para Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) para as políticas de reunião de equipas. 
    - Reveja a [documentação de *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.

