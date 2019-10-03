---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376777"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Controle as configurações do lobby e nível de participação

Essas configurações controlam quais participantes da reunião esperam no lobby antes de serem admitidos na reunião e o nível de participação que são permitidos em uma reunião. Você pode usar o PowerShell para atualizar as configurações de diretiva de reunião que ainda não foram implementadas (rotuladas como "em breve") no centro de administração de equipes.  Veja abaixo um exemplo de cmdlet do PowerShell que permite que todos os usuários ignorem o lobby.  

- [Admitir automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) que as pessoas são uma política por organizador que controla se as pessoas ingressem diretamente em uma reunião ou aguardem no lobby até que sejam admitidas por um usuário autenticado.

- [Permitir que pessoas anônimas iniciem uma reunião](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) é uma política por organizador que controla se pessoas anônimas, incluindo B2B e usuários federados, podem ingressar na reunião do usuário sem um usuário autenticado da organização no atendimento.

- [Permitir que os usuários de discagem ignorem o lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (em**breve**) é uma política por organizador que controla se as pessoas que discar por telefone ingressar na reunião diretamente ou aguardar no lobby, independentemente da configuração de **pessoas automaticamente admitir** .

- [Permitir que os organizadores substituam as configurações do lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**em breve**) é uma política por organizador que controla se o organizador da reunião pode substituir as configurações do lobby que um administrador definir em **admitir automaticamente as pessoas** e **permitir discagem usuários para ignorar o lobby** quando eles agendar uma nova reunião.

**Nota:** Leia [gerenciar diretivas de reunião em equipes](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) para obter uma visão geral completa das diretivas de reunião do Microsoft Teams. 


**Exemplo do PowerShell**

Se você quiser permitir que todos, incluindo usuários externos ou anônimos, ignorem o lobby, você também pode usar o PowerShell para realizar essa tarefa.  Veja um exemplo de como modificar a política de reunião global para sua organização.   

(Certifique-se de rever a documentação acima antes de fazer essas alterações para entender exatamente o que isso permite.)

Set-CsTeamsMeetingPolicy-Identity global-Autoadmitedusers "Everyone"-AllowPSTNUsersToBypassLobby $True

Para obter mais informações, consulte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
