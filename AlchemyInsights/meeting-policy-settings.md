---
title: Definições da política de reunião
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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925176"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gerir políticas de reunião no Microsoft Teams

**Nota: pode demorar até 24 horas para que as alterações de política entrem em vigor para os utilizadores.** Poderá não ser possível fazer alterações de imediato a novas políticas criadas; aguarde 4 horas e tente modificar uma política criada novamente.

As políticas de reunião são utilizadas para controlar as funcionalidades que estão disponíveis aos participantes da reunião para as reuniões agendadas pelos utilizadores na sua organização. Algumas funcionalidades das políticas de reunião podem ainda Teams ser implementadas no centro de administração do Teams (estas funcionalidades são rotuladas como "brevemente" na documentação). Neste caso, ou se estiver a obter um erro como "Não é possível atualizar a política neste momento mas tentar novamente mais tarde" no centro de administração do Microsoft Teams, recomendamos que utilize o PowerShell para criar ou modificar políticas de reunião do Teams. 

Para obter mais informações sobre políticas de reunião, consulte os seguintes recursos:

- Para saber mais sobre como criar políticas, fazer alterações e atribuir utilizadores à política, consulte Gerir políticas de reunião [no Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Para fazer alterações de política através de cmdlets do PowerShell, [consulte a Teams Geral do PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Tem de utilizar o módulo [Skype para Empresas PowerShell para utilizar](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) as Teams de reunião. 
    - [Reveja a documentação dos cmdlets *-CsTeamsMeetingPolicy para](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) obter mais informações.

