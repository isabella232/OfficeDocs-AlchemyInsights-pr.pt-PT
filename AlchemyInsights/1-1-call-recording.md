---
title: Gravação da chamada entre duas pessoas
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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314395"
---
# <a name="11-call-recording"></a>Gravação da chamada entre duas pessoas

Se o **botão Iniciar** Gravação estiver a cinzento numa chamada entre duas pessoas, tem de alterar as definições da política do utilizador afetado. Para verificar a definição da política, execute o Diagnóstico do utilizador afetado ao escrever **Diag: Teams gravação de chamadas 1:1** acima.     

A partir de 31 de maio de 2021, começaremos Teams a impor uma nova política de *chamadas AllowCloudRecordingForCalls*. Antes desta alteração, a gravação de chamadas entre duas pessoas é controlada pela Política de Gravação Teams *AllowCloudRecording.* Esta alteração está documentada na mensagem do Centro de Mensagens: [(Atualizada) 1:1 Introdução à política de gravação de chamadas.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   a opção de política de chamadas está definida **como $False** predefinida. Se preferir bloquear todos os utilizadores de gravar chamadas entre duas pessoas, não precisa de fazer nada.  

Para ativar a gravação de chamadas para todos os utilizadores em chamadas entre [duas pessoas, utilize Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) para executar o seguinte cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Em alternativa, pode criar uma nova política e definir **-AllowCloudRecordingForCalls** para **$true** e atribuir essa política aos seus utilizadores. 

Para obter mais informações, consulte 1:1 Os Controlos da Política de Gravação de [Chamadas estão (Quase!) Aqui.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
