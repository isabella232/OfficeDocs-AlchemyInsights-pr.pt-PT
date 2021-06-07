---
title: Gerir o registo de webinars
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793911"
---
# <a name="manage-webinar-registration"></a>Gerir o registo de webinars

Pode gerir quem pode registar-se Teams Webinars ao utilizar Teams comandos do PowerShell. Para instalar Teams PowerShell, consulte o [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Por *predefinição, o WhoCanRegister* está ativado e definido para **EveryoneInCompany.** Para permitir que qualquer pessoa, incluindo utilizadores anónimos, se registe, tem de definir a Política de Reunião para Todos utilizando o comando do PowerShell: 

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Nota:** se a associação anónima estiver desligada nas definições da reunião, os utilizadores anónimos não podem participar em webinars. Para saber mais e ativar esta definição, consulte [Gerir definições de reunião no Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Se quiser destivar o registo de reuniões, *defina AllowMeetingRegistration* como **Falso.**

Para saber mais sobre como configurar quem pode registar-se em webinars, consulte Configurar quem pode registar-se [em webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obter mais informações sobre as definições das Listas Microsoft, consulte [Definições de controlo para o Microsoft Lists.](/sharepoint/control-lists)
