---
title: Configurações de política de reunião
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
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376772"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerenciar diretivas de reunião no Microsoft Teams

As diretivas de reunião são usadas para controlar os recursos que estão disponíveis para os participantes da reunião para reuniões agendadas por usuários em sua organização. Alguns recursos das diretivas de reunião podem não ser implementados no centro de administração do teams ainda (eles são rotulados "em breve" na documentação). Nesse caso, ou se você estiver recebendo um erro como "não é possível atualizar a diretiva agora, mas tente novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que você use o PowerShell para criar ou modificar as diretivas de reunião de equipes. 

Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre como criar políticas, fazer alterações e atribuir usuários à política, consulte [gerenciar políticas de reunião em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Para fazer alterações de política usando cmdlets do PowerShell, consulte [visão geral do PowerShell de equipes](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Você precisa usar o [Skype para o módulo do PowerShell de negócios](https://www.microsoft.com/download/details.aspx?id=39366) para as diretivas de reunião de equipes. 
    - Revise a [documentação de cmdlets *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obter mais informações.

**Nota:** Pode demorar até 24 horas para que as alterações de política tenham efeito para os utilizadores. Você pode não ser capaz de fazer alterações em diretivas recém-criadas imediatamente; Aguarde 4 horas e tente modificar novamente uma política recém-criada. Se você ainda estiver tendo problemas, tente PowerShell.  