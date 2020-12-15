---
title: Ferramenta de diagnóstico de serviço para Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680228"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b8fd0-102">Ferramenta de diagnóstico de serviço para Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="b8fd0-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b8fd0-103">O Windows Virtual Desktop (WVD) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros através de uma única interface.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b8fd0-104">Esta ferramenta regista informações relacionadas com diagnósticos sempre que a WVD é usada por alguém que atribui um papel de WVD.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b8fd0-105">Cada registo contém informações sobre o papel da WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e a informação sobre o inquilino e utilizador.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b8fd0-106">O Azure Log Analytics pode ser configurado para capturar o registo de atividade criado pela ferramenta de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="b8fd0-107">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="b8fd0-107">Here's how:</span></span>

1. <span data-ttu-id="b8fd0-108">Crie um espaço de trabalho Log Analytics com o [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="b8fd0-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="b8fd0-109">[Ligue os computadores Windows ao Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="b8fd0-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b8fd0-110">Obtenha o ID do espaço de trabalho e a chave primária do seu espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b8fd0-111">O assistente de configuração necessita desta informação para configurar corretamente o agente e garantir que pode comunicar com o Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="b8fd0-112">[Empurre os dados de diagnóstico para o seu espaço de trabalho.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="b8fd0-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b8fd0-113">Pode empurrar os dados de diagnóstico do seu inquilino WVD para o Log Analytics para o seu espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="b8fd0-114">[Identificar e diagnosticar problemas internos](https://go.microsoft.com/fwlink/?linkid=2128338) ou externos em relação à WVD.</span><span class="sxs-lookup"><span data-stu-id="b8fd0-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b8fd0-115">Para saber mais sobre a configuração da ferramenta de diagnóstico de serviço para WVD, consulte [Use Log Analytics para a funcionalidade de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="b8fd0-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
