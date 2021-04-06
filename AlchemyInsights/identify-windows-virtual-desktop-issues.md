---
title: Identificar problemas de ambiente de trabalho virtual do Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595856"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="0c9fb-102">Identificar problemas de ambiente de trabalho virtual do Windows</span><span class="sxs-lookup"><span data-stu-id="0c9fb-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="0c9fb-103">O Windows Virtual Desktop Diagnostics utiliza apenas um cmdlet PowerShell, mas contém muitos parâmetros opcionais para ajudar a reduzir e isolar problemas.</span><span class="sxs-lookup"><span data-stu-id="0c9fb-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="0c9fb-104">Para começar:</span><span class="sxs-lookup"><span data-stu-id="0c9fb-104">To get started:</span></span> 

1. <span data-ttu-id="0c9fb-105">Descarregue e importe o módulo PowerShell virtual do Windows Desktop.</span><span class="sxs-lookup"><span data-stu-id="0c9fb-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="0c9fb-106">Para mais informações, consulte [os Cmdlets de Ambiente de Trabalho Virtual do Windows para Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="0c9fb-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="0c9fb-107">Execute o seguinte cmdlet para iniciar scontabilidade na sua conta:</span><span class="sxs-lookup"><span data-stu-id="0c9fb-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="0c9fb-108">Exemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="0c9fb-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="0c9fb-109">**NOTA:** Todas as consultas que utilizem o PowerShell devem incluir os parâmetros -UserName ou -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="0c9fb-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="0c9fb-110">Para monitorizar as capacidades, consulte Use [Log Analytics para a função de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="0c9fb-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="0c9fb-111">Para filtrar as atividades de diagnóstico pelo utilizador, executar o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="0c9fb-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="0c9fb-112">Exemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="0c9fb-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="0c9fb-113">Há uma lista de filtros que podes correr para diagnosticar problemas.</span><span class="sxs-lookup"><span data-stu-id="0c9fb-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="0c9fb-114">Para saber mais sobre o diagnóstico de problemas, consulte [identificar e diagnosticar problemas de Ambiente de Trabalho Virtual do Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="0c9fb-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="0c9fb-115">Para saber mais sobre erros comuns, consulte [os senarios de erros comuns.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="0c9fb-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
