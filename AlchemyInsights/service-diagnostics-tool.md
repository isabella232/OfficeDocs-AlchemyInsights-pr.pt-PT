---
title: Ferramenta de diagnóstico de serviço para Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595863"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Ferramenta de diagnóstico de serviço para Windows Virtual Desktop

O Windows Virtual Desktop (WVD) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros através de uma única interface. Esta ferramenta regista informações relacionadas com diagnósticos sempre que a WVD é usada por alguém que atribui um papel de WVD. Cada registo contém informações sobre o papel da WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e a informação sobre o inquilino e utilizador. O Azure Log Analytics pode ser configurado para capturar o registo de atividade criado pela ferramenta de diagnóstico seguindo estes passos:

1. Crie um espaço de trabalho Log Analytics com o [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Ligue os computadores Windows ao Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Obtenha o ID do espaço de trabalho e a chave primária do seu espaço de trabalho. O assistente de configuração necessita desta informação para configurar corretamente o agente e garantir que pode comunicar com o Azure Monitor.

1. [Empurre os dados de diagnóstico para o seu espaço de trabalho.](https://go.microsoft.com/fwlink/?linkid=2128284) Pode empurrar os dados de diagnóstico do seu inquilino WVD para o Log Analytics para o seu espaço de trabalho.

1. [Identificar e diagnosticar](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas internos ou externos em relação à WVD.

Para saber mais sobre a configuração da ferramenta de diagnóstico de serviço para WVD, consulte Use Log Analytics para a funcionalidade de diagnóstico.