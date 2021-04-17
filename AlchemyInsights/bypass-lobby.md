---
title: Lobby de bypass
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820045"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Definições de lobby de controlo e nível de participação em equipas

Se quiser permitir que todos, incluindo utilizadores de acesso de marcação, externos e anónimos, **contornem o lobby,** utilize o PowerShell para realizar esta tarefa. Aqui está um exemplo de modificar a política global de reuniões para a sua organização.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Este cmdlet requer atualmente a utilização do Módulo Skype para Business PowerShell. Para se preparar para utilizar este cmdlet, consulte [as políticas de gestão via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Uma vez configurada uma política, tem de a aplicar aos utilizadores; ou, se modificar a política Global, aplicar-se-á automaticamente aos utilizadores. Para qualquer mudança de política, é necessário esperar pelo menos **4 horas até 24 horas** para que as políticas entrem em vigor. 

Certifique-se de rever a documentação abaixo antes de então fazer estas alterações para entender exatamente o que isso permite.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Equipas compreensivas que reúnem controlos políticos de lobby

Estas definições controlam quais os participantes que se encontram aguardam no átrio antes de serem admitidos na reunião e do nível de participação que lhes é permitido numa reunião. Pode utilizar o PowerShell para atualizar as definições de política de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração das Equipas. Veja abaixo um exemplo PowerShell cmdlet que permite a todos os utilizadores contornar o lobby.

- [Admitir automaticamente as pessoas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) é uma política por organizador que controla se as pessoas se juntam a uma reunião diretamente ou esperam no lobby até serem admitidas por um utilizador autenticado.

- [Permitir que pessoas anónimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anónimas, incluindo B2B e utilizadores federados, podem participar na reunião do utilizador sem um utilizador autenticado da organização presente.

- [Permitir que os utilizadores de acesso telefónico contornem o lobby (em](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **breve**) é uma política por organizador que controla se as pessoas que ligam por telefone se juntam diretamente à reunião ou esperam no lobby **independentemente** da configuração automática de pessoas.

- [Permitir que os organizadores substituam as definições de lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(em breve**) é uma política por organizador que controla se o organizador da reunião pode sobrepor as definições do lobby que um administrador definido em Automaticamente **admitem pessoas** e **permitem que os utilizadores de acesso de marcação contornem o lobby** quando agendam uma nova reunião.

**Nota:** Leia [Gerir as políticas de reunião em Equipas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para uma visão geral completa das políticas de reunião das Equipas da Microsoft.
