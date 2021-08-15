---
title: Aumente a tecnologia NDI
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023533"
---
# <a name="turn-on-ndi-technology"></a>Aumente a tecnologia NDI

A tecnologia NDI requer que um utilizador tenha dois passos:

1. O administrador de inquilinos tem de ativar a propriedade "AllowNDIStreaming" no CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Após esta alteração ter sido preenchida, o utilizador final terá de ativos a tecnologia NDI® no seu cliente específico **a partir Definições > Permissões.**

Para obter mais informações, [consulte Utilizar tecnologia NDI no Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
