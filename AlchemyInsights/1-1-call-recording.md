---
title: 1:1 gravação de chamada
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733860"
---
# <a name="11-call-recording"></a>1:1 gravação de chamada

Os administradores precisam de tomar medidas agora para continuar a permitir que os utilizadores gravem chamadas 1:1.
 
A partir de 12 de abril de 2021, começaremos a aplicar uma nova opção de Política de Chamadas de Equipas *AllowCloudRecordingForCalls*. 

Atualmente, as capacidades de gravação de chamadas 1:1 são controladas pela opção *AllowCloudRecording* em Políticas de Reunião de Equipas. Se os seus utilizadores estiverem autorizados a gravar Reuniões de Equipas, também podem gravar chamadas de 1:1.

Se preferir bloquear todos os utilizadores de gravar chamadas 1:1, não precisa de tomar nenhuma ação. A opção de chamada *AllowCloudRecordingForCalls* será $False por padrão.

Esta alteração está documentada no seguinte Post do Centro de Mensagens: [(Atualizado) 1:1 Introdução da política de gravação de chamadas](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Para definir a opção política de chamada de equipas deve utilizar o [PowerShell das Equipas](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Para ativar a gravação de chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identidade Global -AllowCloudRecordingForCalls $True

**Para desativar a gravação de chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identidade Global -AllowCloudRecordingForCalls $False

