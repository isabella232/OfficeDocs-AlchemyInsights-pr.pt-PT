---
title: Problemas de desempenho do Microsoft Defender para Ponto Final no Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794001"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemas de desempenho do Microsoft Defender para Ponto Final no Linux

Este artigo guia-o ao longo dos passos de identificação de problemas de desempenho do Microsoft Defender para Endpoint no Linux.

Primeiro, é importante verificar se o problema que está a ter foi resolvido com a versão [mais recente.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Para iniciar a sua investigação, consulte [Remoção de problemas de desempenho do Microsoft Defender para Endpoint no Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Exclusões

As exclusões podem ajudar a mitigar problemas de desempenho. Reveja as suas exclusões antes de começar para que qualquer risco adicional seja conhecido e documentado.

Para obter mais informações, consulte [Configurar e validar exclusões do Microsoft Defender para Pontos Finais no Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Quando tiver múltiplos ficheiros & pastas a excluir e se encontrarem todos no mesmo ponto de montagem, poderá ser mais fácil excluir o ponto de montagem. A partir do lançamento de fevereiro 101.22.80, pode excluir uma montagem inteira.

Por exemplo, se /mnt/backup for um ponto de montagem, pode adicionar /mnt/backup à lista de exclusões ao executar este comando:

`$ mdatp exclusion folder add –path /mnt/backup`

**Nota:** adicionar exclusões aumenta o risco de o software malicado não ser detetado e deve ser tratado e implementado com cuidado.

## <a name="need-help"></a>Precisa de Ajuda?

Para o ajudar da forma mais eficiente, recolha os dados de diagnóstico antes de abrir um caso de suporte.
