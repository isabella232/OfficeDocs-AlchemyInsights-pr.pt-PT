---
title: Como ativar o Correio de Voz hospedado
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679169"
---
# <a name="how-to-enable-hosted-voicemail"></a>Como ativar o Correio de Voz hospedado

Para ativar o Correio de Voz, **o HostedVoicemail** tem de ser definido para $true.

A propriedade **HostedVoicemail** no utilizador utilizando Remote PowerShell (RPS).

Para obter mais informações sobre a ligação ao RPS, consulte a [Visão Geral powershell das equipas da Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre a ligação ao RPS.

1. O Administrador das Equipas deve ser registado no Remote PowerShell para equipas.
1. A partir do PowerShell, o Teams Admin pode executar **set-csuser user@contoso.com -HostedVoiceMail $true** onde o sip uri é do utilizador em questão.

> [!NOTE]
> As alterações às políticas podem demorar até 24 horas a replicar-se.