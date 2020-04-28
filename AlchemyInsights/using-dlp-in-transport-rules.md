---
title: Usar DLP em regras de transporte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915190"
---
# <a name="using-dlp-in-transport-rules"></a>Usar DLP em regras de transporte

Para integrar a Prevenção de Perdas de Dados (DLP) num transporte existente, use a condição "**Se a mensagem contiver... Informações Confidenciais**" na definição da regra de Transporte.

**Para obter mais detalhes, consulte:**

- Tipos de DLP de informação confidencial integrados em regras de transporte: [Integrar Regras de Informação Confidencial](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Pode também testar a regra com ou sem teste de política ao usar o Modo de Teste na regra.  Depois de ter criado a regra, deve esperar 30 minutos antes de a testar.

- Consulte [Testar regras de Fluxo de E-mail/Transporte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).

**Nota**: se estiver a tentar implementar uma nova política de DLP com regras de transporte no EAC, use, ao invés, [Políticas DLP no centro de Segurança e Conformidade](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
