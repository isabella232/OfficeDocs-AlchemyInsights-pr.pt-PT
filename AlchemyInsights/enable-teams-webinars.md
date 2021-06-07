---
title: Ativar Teams Webinars
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793782"
---
# <a name="enable-teams-webinars"></a>Ativar Teams Webinars

Os webinars estão ativados por predefinição. Pode gerir quem pode agendar e registar-se em Webinars Teams utilizando Teams comandos do PowerShell.

- Todos os utilizadores que podem criar uma reunião também podem criar uma reunião de webinar. Se quiser gerir quem pode agendar Webinars Teams, utilize *AllowMeetingRegistration.* 
- Por *predefinição, o WhoCanRegister* está ativado e definido como **Todos.** Se quiser destivar o registo de reuniões, *defina AllowMeetingRegistration* como **Falso.**

Para alterar estas definições, tem de instalar o [Teams PowerShell.](/microsoftteams/teams-powershell-install) Além disso, as Políticas de Reunião são impodas Teams webinars. Por exemplo, se a associação anónima estiver desligada nas definições da reunião, os utilizadores anónimos não podem participar em webinars.

Para saber mais sobre como configurar quem pode registar-se em webinars, consulte Configurar quem pode registar-se [em webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obter mais informações sobre as definições das Listas Microsoft, consulte [Definições de controlo para o Microsoft Lists.](/sharepoint/control-lists)