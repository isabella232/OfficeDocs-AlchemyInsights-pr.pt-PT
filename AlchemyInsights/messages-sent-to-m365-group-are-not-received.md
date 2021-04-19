---
title: As mensagens enviadas para o grupo do Microsoft 365 não são recebidas por todos os membros
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823798"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>As mensagens enviadas para um grupo do Microsoft 365 não são recebidas por todos os membros

Certifique-se de que todos os membros do grupo subscreveram a receção dos e-mails. Consulte [Seguir um grupo no Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Para verificar o estado da mensagem dos membros que subscreveram os e-mails do grupo, execute o seguinte comando no [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Utilize o seguinte comando do EXO PowerShell para configurar todos os membros do grupo a fim de receberem e-mails enviados para o grupo do Microsoft 365 na respetiva caixa de entrada:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Por exemplo:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`