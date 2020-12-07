---
title: O ícone do calendário não está a aparecer no cliente da Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583923"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>O ícone do calendário não está a aparecer no cliente da Microsoft Teams

O **Separador de Calendário** em Equipas requer acesso a uma caixa de correio de troca através de Serviços Web de Câmbio. A caixa de correio da Exchange pode ser Online ou No-Local. Para os utilizadores online que não vêem o **Separador calendário,** certifique-se de que [estão licenciados para uma caixa de correio Exchange Online e a caixa de correio está ativada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Se os seus utilizadores estiverem a bordo no Local, tem de confirmar que a sua configuração Híbrida é saudável. Utilize o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para resolver problemas. Tenha em conta que o [Teams necessita do Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Para obter mais informações e etapas de resolução de problemas, consulte [problemas de interação com as Equipas da Microsoft e o Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
