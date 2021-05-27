---
title: A remoção de problemas de deteção de problemas deteção de erros
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676279"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>A remoção de problemas de deteção de problemas deteção de erros

Está a ter problemas com as deteções de e-? Eis algumas práticas recomendadas a ter em conta:

- Verifique o estado da distribuição em espera.  Se o estado estiver **Atual (Pendente)** ou **Desativado (Pendente),** aguarde até que a distribuição em suspensão seja concluída.
- Intercalie as atualizações da Deteção de Dados Eletrões num único pedido em massa em vez de atualizar a política repetidamente para cada transação.
- Execute Set-CaseHoldPolicy <policyname> -RetryDistribution no PowerShell do Centro de Conformidade e Segurança. Para obter detalhes, consulte [Ligação Centro de Conformidade & PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Para obter os passos para verificar estas definições e práticas recomendadas adicionais para a mitigação e resolução de problemas de Deteção de Dados Técnicos, consulte Resolução de problemas de erros de deteção de [dados técnicos.](/microsoft-365/compliance/hold-distribution-errors)
Para mais informações sobre a resolução de outros problemas comuns na Deteção de Dados Online, consulte Investigar, resolver problemas e resolver problemas comuns na Deteção [de Dados Dados Online.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
