---
title: Política de proteção de aplicações
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423964"
---
# <a name="application-protection-policy"></a>Política de proteção de aplicações

Se é novo na política de proteção de aplicações (APP), consulte a visão geral das [políticas de proteção](https://docs.microsoft.com/intune/apps/app-protection-policy)da App.

Para começar a utilizar a APP, consulte [Como criar e atribuir políticas de proteção de aplicações.](https://docs.microsoft.com/intune/app-protection-policies)

Requisitos da política de proteção de aplicações:

- O utilizador tem uma licença Intune ou EMS.
- O utilizador pertence a um grupo visado pelas políticas de proteção de aplicações.
- Apenas um utilizador corporativo é assinado em aplicações protegidas num dispositivo.
- A aplicação implementou o [Intune SDK.](https://docs.microsoft.com/intune/app-sdk-get-started) Para obter uma lista de aplicações que suportam o SDK, consulte [as aplicações protegidas do Microsoft Intune.](https://docs.microsoft.com/intune/apps-supported-intune-apps)

As políticas aplicam-se depois de um utilizador que satisfaça os sinais acima referidos numa aplicação ativada pelo Intune SDK. A forma mais fácil de determinar se uma apólice é aplicada é exigindo que o utilizador estabeleça um pino na apólice. 

Para obter mais informações, consulte:

[APP/MAM resolução de problemas faQ](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Como validar a configuração da sua política de proteção de aplicações](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Compreender o tempo de entrega da Política de Proteção de Aplicações](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Como monitorizar as políticas de proteção de aplicações](https://docs.microsoft.com/intune/app-protection-policies-monitor)