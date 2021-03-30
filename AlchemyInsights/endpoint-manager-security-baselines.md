---
title: EndPoint Manager - Linhas de base de segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421087"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Linhas de base de segurança

As linhas de base de segurança são grupos pré-configurados de definições do Windows que o ajudam a aplicar as definições de segurança recomendadas pelas equipas de segurança relevantes. Estas linhas de base podem ser personalizadas para fornecer apenas as configurações e valores desejados. Para obter mais informações sobre linhas de segurança, consulte [utilize linhas de base de segurança para configurar dispositivos Windows 10 no Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Existem atualmente linhas de base para estes produtos:

- Definições de segurança DO Windows MDM
- Microsoft Defender para Segurança EndPoint
- Microsoft Edge

Cada uma das linhas de base é atualizada periodicamente e lançada em versões incrementais. Cada versão adiciona e remove as definições da versão anterior para garantir que a linha de base satisfaz a orientação atual. A consola de bases de segurança em Endpoint Security permite comparar diferentes versões, tornando visíveis as alterações da versão para a versão.

Para obter orientações sobre como alterar de forma mais eficaz qual a versão de linha de base implementada, consulte [Gerir os perfis de base de segurança no Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Depois de implementar uma linha de base de segurança, pode monitorizar o estado de implementação e revisão das definições numa base dispositivo por dispositivo.

**Nota:** Os dados de reporte das linhas de base podem demorar até 24 horas a aparecer desde a implantação inicial a um dispositivo e até 6 horas para novas atualizações. 

A causa mais comum de uma definição de linha de base não aplicada é porque a mesma definição está sendo usada num perfil diferente. Este cenário pode ser investigado para dispositivos específicos selecionando esse dispositivo a partir do nó de Estado do Dispositivo do perfil base de segurança. Para mais detalhes, consulte [resolver conflitos para linhas de base de segurança](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).