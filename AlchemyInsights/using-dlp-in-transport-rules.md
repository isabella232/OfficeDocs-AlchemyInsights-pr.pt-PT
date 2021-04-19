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
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827227"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="0adc8-102">Usar DLP em regras de transporte</span><span class="sxs-lookup"><span data-stu-id="0adc8-102">Using DLP in transport rules</span></span>

<span data-ttu-id="0adc8-103">Para integrar a Prevenção de Perdas de Dados (DLP) num transporte existente, use a condição "**Se a mensagem contiver... Informações Confidenciais**" na definição da regra de Transporte.</span><span class="sxs-lookup"><span data-stu-id="0adc8-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="0adc8-104">**Para obter mais detalhes, consulte:**</span><span class="sxs-lookup"><span data-stu-id="0adc8-104">**For more details, see:**</span></span>

- <span data-ttu-id="0adc8-105">Tipos de DLP de informação confidencial integrados em regras de transporte: [Integrar Regras de Informação Confidencial](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="0adc8-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="0adc8-106">Pode também testar a regra com ou sem teste de política ao usar o Modo de Teste na regra.</span><span class="sxs-lookup"><span data-stu-id="0adc8-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="0adc8-107">Depois de ter criado a regra, deve esperar 30 minutos antes de a testar.</span><span class="sxs-lookup"><span data-stu-id="0adc8-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="0adc8-108">Consulte [Testar regras de Fluxo de E-mail/Transporte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).</span><span class="sxs-lookup"><span data-stu-id="0adc8-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="0adc8-109">**Nota**: se estiver a tentar implementar uma nova política de DLP com regras de transporte no EAC, use, ao invés, [Políticas DLP no centro de Segurança e Conformidade](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0adc8-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
