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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318659"
---
# <a name="how-to-enable-hosted-voicemail"></a>Como ativar o Voicemail Alotado

Para ativar o Voicemail, **o HostedVoicemail** tem de estar definido como $true.

A **propriedade HostedVoicemail** do utilizador que utiliza o PowerShell Remoto (RPS).

Para obter mais informações sobre como ligar a RPS, consulte o Microsoft Teams Geral do [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obter mais informações sobre como ligar a RPS.

1. O Teams de Administração do PowerShell deverá ter sessão sessão em PowerShell remoto para Teams.
1. A partir do PowerShell, é pedido ao administrador do Teams que pode executar **set-csuser user@contoso.com -HostedVoiceMail $true** onde o sip uri é do utilizador em questão.

**Nota:** as alterações a políticas podem demorar até 24 horas a replicar.