---
title: Ferramenta de diagnóstico de serviço para Windows Ambiente de Trabalho Virtual
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052397"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Ferramenta de diagnóstico de serviço para Windows Ambiente de Trabalho Virtual

Windows O WVD (Virtual Desktop) oferece uma ferramenta de diagnóstico que permite aos administradores identificar erros através de uma única interface. Esta ferramenta regista informações relacionadas com diagnósticos sempre que o WVD é utilizado por alguém com uma função WVD atribuída. Cada registo contém informações sobre a função WVD envolvida na atividade, as mensagens de erro que são apresentadas durante a sessão e as informações sobre o inquilino e o utilizador. A Análise de Registos do Azure pode ser configurada para capturar o registo de atividade criado pela ferramenta de diagnóstico. Faça o seguinte:

1. Crie uma área de trabalho da Log Analytics com o portal ou [com](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Ligação Windows para o Monitor do Azure.](https://go.microsoft.com/fwlink/?linkid=2129913) Obter o ID da Área de Trabalho e a Chave Primária da sua área de trabalho. O assistente de configuração precisa desta informação para configurar o agente corretamente e para garantir que consegue comunicar com o Monitor do Azure.
1. [Empurrar os dados de diagnóstico para a sua área de trabalho](https://go.microsoft.com/fwlink/?linkid=2128284). Pode push diagnostics data from your WVD tenant to the Log Analytics for your workspace.
1. [Identifique e diagnostice problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos ou externos em relação ao WVD.

Para saber mais sobre como configurar a ferramenta de diagnóstico de serviço para o WVD, consulte o artigo Utilizar Análise de Registos para a [funcionalidade de diagnóstico.](https://go.microsoft.com/fwlink/?linkid=2128084)
