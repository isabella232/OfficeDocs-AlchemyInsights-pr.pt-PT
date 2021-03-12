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
# <a name="11-call-recording"></a><span data-ttu-id="66740-102">1:1 gravação de chamada</span><span class="sxs-lookup"><span data-stu-id="66740-102">1:1 call recording</span></span>

<span data-ttu-id="66740-103">Os administradores precisam de tomar medidas agora para continuar a permitir que os utilizadores gravem chamadas 1:1.</span><span class="sxs-lookup"><span data-stu-id="66740-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="66740-104">A partir de 12 de abril de 2021, começaremos a aplicar uma nova opção de Política de Chamadas de Equipas *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="66740-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="66740-105">Atualmente, as capacidades de gravação de chamadas 1:1 são controladas pela opção *AllowCloudRecording* em Políticas de Reunião de Equipas.</span><span class="sxs-lookup"><span data-stu-id="66740-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="66740-106">Se os seus utilizadores estiverem autorizados a gravar Reuniões de Equipas, também podem gravar chamadas de 1:1.</span><span class="sxs-lookup"><span data-stu-id="66740-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="66740-107">Se preferir bloquear todos os utilizadores de gravar chamadas 1:1, não precisa de tomar nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="66740-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="66740-108">A opção de chamada *AllowCloudRecordingForCalls* será $False por padrão.</span><span class="sxs-lookup"><span data-stu-id="66740-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="66740-109">Esta alteração está documentada no seguinte Post do Centro de Mensagens: [(Atualizado) 1:1 Introdução da política de gravação de chamadas](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Para definir a opção política de chamada de equipas deve utilizar o [PowerShell das Equipas](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="66740-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="66740-110">**Para ativar a gravação de chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identidade Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="66740-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="66740-111">**Para desativar a gravação de chamadas em chamadas 1:1:** Set-CsTeamsCallingPolicy -Identidade Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="66740-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

