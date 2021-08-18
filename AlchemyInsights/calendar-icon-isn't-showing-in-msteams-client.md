---
title: O ícone calendário não é apresentado no Microsoft Teams cliente
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120015"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>O ícone calendário não é apresentado no Microsoft Teams cliente

O **Separador** Calendário no Teams necessita de acesso a uma Exchange correio eletrónico através Exchange Web Services. A Exchange de correio pode ser Online ou No Local. Para utilizadores online que  não veem o separador Calendário, certifique-se de que estão licenciados para uma caixa de correio do Exchange Online e que a caixa de correio [está ativada.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Se os seus utilizadores estiverem abriados no Local, tem de confirmar que a sua configuração Híbrida está em bom estado de gestão. Utilize o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para resolver problemas. Tenha em conta que o [Teams necessita do Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Para obter mais informações e passos de remoção de problemas, consulte o Microsoft Teams problemas [Exchange Server de interação.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
