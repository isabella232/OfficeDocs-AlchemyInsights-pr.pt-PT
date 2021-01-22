---
title: Ligue a tecnologia NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935135"
---
# <a name="turn-on-ndi-technology"></a>Ligue a tecnologia NDI

A tecnologia NDI requer dois passos para ser ligado para um utilizador:

1. O administrador do arrendatário deve permitir a propriedade 'AllowNDIStreaming' em CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Após esta alteração ter sido preenchida, o utilizador final deve ligar a tecnologia NDI® para o seu cliente específico a partir de **Definições > Permissões**.

Para obter mais informações, consulte [a tecnologia NDI em Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
