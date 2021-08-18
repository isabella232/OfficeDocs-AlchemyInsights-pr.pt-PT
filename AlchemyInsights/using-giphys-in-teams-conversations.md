---
title: Utilizar Giphys em Teams Conversações
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323531"
---
# <a name="using-giphys-in-teams-conversations"></a>Utilizar Giphys em Teams Conversações

O acesso giphys em Teams chat está ativado por predefinição. Enquanto administrador, pode controlar se Os Giphys estão disponíveis para os utilizadores ao definir uma política de mensagens e garantir que a definição Utilizar **Giphys** em conversações está **Ativada.** [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)

Se os GIFs não estiverem a funcionar conforme esperado Teams conversações, verifique:

A [política de mensagens tem](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) de permitir Giphys. Para verificar com cmdlets do PowerShell:

- Verifique se pode Gerir [contactos Teams com o PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Execute o comando Do PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verifique se **AllowGiphy** está definido como **VERDADEIRO.**
- Se **AllowGiphy** estiver definido como **FALSO,** execute o seguinte comando do PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[As Experiências Ligadas Opcionais](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) têm de ser ativadas para permitir o acesso ao URL do Giphy.

**Nota:** se tiver múltiplas políticas de mensagens do Teams configuradas para o seu inquilino, pode determinar a identidade da política atribuída ao utilizador afetado com o comando do PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selecione TeamsMessagingPolicy.
