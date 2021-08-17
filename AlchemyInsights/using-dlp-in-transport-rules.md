---
title: Usar DLP em regras de transporte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084105"
---
# <a name="using-dlp-in-transport-rules"></a>Usar DLP em regras de transporte

Para integrar a Prevenção de Perdas de Dados (DLP) num transporte existente, use a condição "**Se a mensagem contiver... Informações Confidenciais**" na definição da regra de Transporte.

**Para obter mais detalhes, consulte:**

- Tipos de DLP de informação confidencial integrados em regras de transporte: [Integrar Regras de Informação Confidencial](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Pode também testar a regra com ou sem teste de política ao usar o Modo de Teste na regra.  Depois de ter criado a regra, deve esperar 30 minutos antes de a testar.

- Consulte [Testar regras de Fluxo de E-mail/Transporte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).

**Nota**: se estiver a tentar implementar uma nova política de DLP com regras de transporte no EAC, use, ao invés, [Políticas DLP no centro de Segurança e Conformidade](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
