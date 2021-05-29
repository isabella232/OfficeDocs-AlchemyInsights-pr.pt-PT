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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702101"
---
# <a name="11-call-recording"></a><span data-ttu-id="fc523-102">Gravação da chamada entre duas pessoas</span><span class="sxs-lookup"><span data-stu-id="fc523-102">1:1 call recording</span></span>

<span data-ttu-id="fc523-103">Se o **botão Iniciar** Gravação estiver a cinzento numa chamada entre duas pessoas, tem de alterar as definições da política do utilizador afetado.</span><span class="sxs-lookup"><span data-stu-id="fc523-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="fc523-104">Para verificar a definição de política, execute o Diagnóstico do utilizador afetado ao escrever **Diag: Teams 1:1 Gravação de Chamadas** acima.</span><span class="sxs-lookup"><span data-stu-id="fc523-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="fc523-105">A partir de 31 de maio de 2021, começaremos Teams a impor uma nova política de *chamadas AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="fc523-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="fc523-106">Antes desta alteração, a gravação de chamadas entre duas pessoas é controlada pela Política de Registo de Alterações Teams *AllowCloudRecording.*</span><span class="sxs-lookup"><span data-stu-id="fc523-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="fc523-107">Esta alteração está documentada na mensagem do Centro de Mensagens: [(Atualizada) 1:1 Introdução à política](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)de gravação de chamadas .</span><span class="sxs-lookup"><span data-stu-id="fc523-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="fc523-108">*AllowCloudRecordingForCalls*   a opção de política de chamadas está definida **como $False** predefinida.</span><span class="sxs-lookup"><span data-stu-id="fc523-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="fc523-109">Se preferir bloquear todos os utilizadores de gravar chamadas entre duas pessoas, não precisa de fazer nada.</span><span class="sxs-lookup"><span data-stu-id="fc523-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="fc523-110">Para ativar a gravação de chamadas para todos os utilizadores em chamadas entre [duas pessoas, utilize Teams PowerShell](/microsoftteams/teams-powershell-install) para executar o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="fc523-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="fc523-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="fc523-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="fc523-112">Em alternativa, pode criar uma nova política e definir **-AllowCloudRecordingForCalls** para **$true** e atribuir essa política aos seus utilizadores.</span><span class="sxs-lookup"><span data-stu-id="fc523-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="fc523-113">Para obter mais informações, consulte 1:1 Os Controlos da Política de Gravação de [Chamadas estão (Quase!) Aqui.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="fc523-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
