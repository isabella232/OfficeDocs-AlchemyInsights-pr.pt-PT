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
# <a name="identify-windows-virtual-desktop-issues"></a>Identificar problemas de ambiente de trabalho virtual do Windows

O Windows Virtual Desktop Diagnostics utiliza apenas um cmdlet PowerShell, mas contém muitos parâmetros opcionais para ajudar a reduzir e isolar problemas. Para começar: 

1. Descarregue e importe o módulo PowerShell virtual do Windows Desktop. Para mais informações, consulte [os Cmdlets de Ambiente de Trabalho Virtual do Windows para Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Execute o seguinte cmdlet para iniciar scontabilidade na sua conta:
    
    Exemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NOTA:** Todas as consultas que utilizem o PowerShell devem incluir os parâmetros -UserName ou -ActivityID. Para monitorizar as capacidades, consulte Use [Log Analytics para a função de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).

Para filtrar as atividades de diagnóstico pelo utilizador, executar o seguinte cmdlet:

Exemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Há uma lista de filtros que podes correr para diagnosticar problemas. Para saber mais sobre o diagnóstico de problemas, consulte [identificar e diagnosticar problemas de Ambiente de Trabalho Virtual do Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Para saber mais sobre erros comuns, consulte [os senarios de erros comuns.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
