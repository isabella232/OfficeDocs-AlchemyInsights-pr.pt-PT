---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821458"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="c957f-102">Corrigir problemas de entrega para código de erro 550 5.4.1 Relé De acesso negado</span><span class="sxs-lookup"><span data-stu-id="c957f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="c957f-103">Este problema ocorre [ao verificar se um endereço de e-mail é válido para evitar retornos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede microsoft.</span><span class="sxs-lookup"><span data-stu-id="c957f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="c957f-104">Experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c957f-104">Try the following:</span></span>

1. <span data-ttu-id="c957f-105">Determinar se o problema é específico de todo um domínio ou de um único endereço de e-mail:</span><span class="sxs-lookup"><span data-stu-id="c957f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="c957f-106">Domínio inteiro: Por vezes, o domínio precisa de ser sincronizado; tente [definir o domínio para Interno e, em seguida, de volta para Autoritário](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="c957f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="c957f-107">Endereço de e-mail único: Por vezes, o endereço precisa de ser sincronizado; mudar o endereço de procuração smtp e, em seguida, mudá-lo de volta pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="c957f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="c957f-108">Determinar se o problema é específico de um grupo ou de uma pasta pública.</span><span class="sxs-lookup"><span data-stu-id="c957f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="c957f-109">Para alguns tipos de objetos, os objetos podem ter de ser criados manualmente no Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="c957f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="c957f-110">Se precisar de ajuda adicional, abra um bilhete de apoio e especifique o âmbito do problema (incluindo o tipo de objeto que está a enviar) para que possamos ajudá-lo melhor.</span><span class="sxs-lookup"><span data-stu-id="c957f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>