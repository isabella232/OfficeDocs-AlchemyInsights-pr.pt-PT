---
title: O ícone do Calendário não é apresentado no cliente do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989602"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>O ícone do Calendário não é apresentado no cliente do Teams

O separador Calendário no Teams necessita de acesso a uma caixa de correio do Exchange através dos Serviços Web Exchange. A caixa de correio do Exchange pode estar Online ou No Local. Para utilizadores Online que não vejam o separador Calendário, certifique-se de que [têm licença para uma caixa de correio Exchange Online e que a caixa de correio está ativada](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Se o utilizador tiver uma caixa de correio válida no Exchange Online, mas ainda não conseguir ver o separador Calendário, poderá estar a ter um problema de rede. Utilize o [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) e execute os **Testes de Conectividade dos Serviços Web do Microsoft Exchange** para o utilizador afetado.

Por último, consulte as [Políticas de configuração de aplicações nas Aplicações do Teams](https://admin.teams.microsoft.com/policies/app-setup) para garantir que a aplicação Calendário não foi removida da política aplicada ao utilizador (provavelmente a **Global (predefinição da organização)**.

Se os seus utilizadores estiverem alojados No Local, precisa de confirmar que a sua Configuração híbrida tem bom estado de funcionamento. Utilize o [Assistente de Configuração Híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para resolver problemas.

Tenha em conta que o [Teams necessita do Exchange 2016 CU3 ou superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
