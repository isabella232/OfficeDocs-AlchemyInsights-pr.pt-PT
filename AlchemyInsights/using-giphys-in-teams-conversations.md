---
title: Usando Giphys em conversas de equipas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982581"
---
# <a name="using-giphys-in-teams-conversations"></a>Usando Giphys em conversas de equipas

O acesso de Giphys no chat de Equipas é ativado por padrão. Como administrador, pode controlar se o Giphys estiver disponível para os [utilizadores, definindo uma política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) e garantindo que **o Uso de Giphys nas conversas** é **On**.

Se os GIFs não estiverem a funcionar como esperado nas conversas das equipas, verifique:

A [política de mensagens](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) tem de permitir o Giphys. Para verificar utilizando cmdlets PowerShell:

- Verifique se consegue [gerir equipas com PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Executar o comando PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verificar se **AllowGiphy** está definido para **TRUE**.
- Se **o AllowGiphy** estiver definido como **FALSE,** executar o seguinte comando PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[As experiências conectadas opcionais](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) devem ser ativadas para permitir o acesso ao URL giphy.

> [!NOTE]
> Se tiver várias políticas de mensagens de equipas configuradas para o seu inquilino, pode determinar a identidade da política atribuída ao utilizador impactado com o comando PowerShell [Get-CsOnlineUser -Identidade](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> ; Selecione TeamsMessagingPolicy.
