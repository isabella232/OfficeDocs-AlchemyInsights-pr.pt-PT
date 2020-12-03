---
title: Erro de licenciamento DLP de endpoint
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564865"
---
# <a name="endpoint-dlp-licensing-error"></a>Erro de licenciamento DLP de ponto final

Ao tentar configurar o Endpoint DLP, se receber o seguinte erro:

`Your organization is missing the licenses required to manage these devices`.

Certifique-se de que tem uma das seguintes subscrições ou add-ons:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Conformidade microsoft 365 E5
- Conformidade microsoft 365 A5
- Microsoft 365 E5 proteção e governação de informação
- Microsoft 365 A5 proteção e governação de informação

> [!NOTE]
> Isto não funcionará para combinações de licenças como: Win E5 + O365 E5 + EMS E5. Você deve ter uma licença M365 E5 pura para configurar esta funcionalidade.

Para obter mais informações sobre o licenciamento endpoint DLP, consulte [o Licenciamento Endpoint DLP.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
