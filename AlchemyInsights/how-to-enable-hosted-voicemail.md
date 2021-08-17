---
title: Como ativar o Voicemail Alotado
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055565"
---
# <a name="how-to-enable-hosted-voicemail"></a>Como ativar o Voicemail Alotado

Para ativar o Voicemail, **o HostedVoicemail** tem de estar definido como $true.

A **propriedade HostedVoicemail** do utilizador que utiliza o PowerShell Remoto (RPS).

Para obter mais informações sobre como ligar a RPS, consulte o Microsoft Teams Geral do [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre como ligar a RPS.

1. O Teams de Administração do Teams deve ter sessão sessão com o PowerShell Remoto.
1. A partir do PowerShell, é pedido ao administrador do Teams que pode executar **o set-csuser user@contoso.com -HostedVoiceMail $true** onde o sip uri é do utilizador em questão.

> [!NOTE]
> As alterações às políticas podem demorar até 24 horas a replicar.