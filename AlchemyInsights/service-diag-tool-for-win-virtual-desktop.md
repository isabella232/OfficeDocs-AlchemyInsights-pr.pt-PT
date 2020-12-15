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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Ferramenta de diagnóstico de serviço para Windows Virtual Desktop

O Windows Virtual Desktop (WVD) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros através de uma única interface. Esta ferramenta regista informações relacionadas com diagnósticos sempre que a WVD é usada por alguém que atribui um papel de WVD. Cada registo contém informações sobre o papel da WVD envolvida na atividade, as mensagens de erro que aparecem durante a sessão e a informação sobre o inquilino e utilizador. O Azure Log Analytics pode ser configurado para capturar o registo de atividade criado pela ferramenta de diagnóstico. Faça o seguinte:

1. Crie um espaço de trabalho Log Analytics com o [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Ligue os computadores Windows ao Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Obtenha o ID do espaço de trabalho e a chave primária do seu espaço de trabalho. O assistente de configuração necessita desta informação para configurar corretamente o agente e garantir que pode comunicar com o Azure Monitor.
1. [Empurre os dados de diagnóstico para o seu espaço de trabalho.](https://go.microsoft.com/fwlink/?linkid=2128284) Pode empurrar os dados de diagnóstico do seu inquilino WVD para o Log Analytics para o seu espaço de trabalho.
1. [Identificar e diagnosticar problemas internos](https://go.microsoft.com/fwlink/?linkid=2128338) ou externos em relação à WVD.

Para saber mais sobre a configuração da ferramenta de diagnóstico de serviço para WVD, consulte [Use Log Analytics para a funcionalidade de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2128084).
