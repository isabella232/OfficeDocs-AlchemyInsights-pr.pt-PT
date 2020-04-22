---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707922"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="33e9b-102">Corrigir problemas de entrega para código de erro 550 5.4.1 Acesso de retransmissão negado</span><span class="sxs-lookup"><span data-stu-id="33e9b-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="33e9b-103">Este problema ocorre ao verificar se um endereço de [e-mail é válido para evitar ressaltos](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ao entrar na rede da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="33e9b-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="33e9b-104">Tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="33e9b-104">Try the following:</span></span>

1. <span data-ttu-id="33e9b-105">Determine se o problema é específico de um domínio inteiro ou de um único endereço de e-mail:</span><span class="sxs-lookup"><span data-stu-id="33e9b-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="33e9b-106">Domínio inteiro: Às vezes o domínio precisa de ser sincronizado; tente [definir o domínio para Interno e, em seguida, de volta ao Authoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="33e9b-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="33e9b-107">Endereço de e-mail único: Às vezes, o endereço precisa de ser sincronizado; mudar o endereço de procuração smtp e, em seguida, mudá-lo de volta pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="33e9b-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="33e9b-108">Determine se o problema é específico de um grupo ou pasta pública.</span><span class="sxs-lookup"><span data-stu-id="33e9b-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="33e9b-109">Para alguns tipos de objetos, os objetos podem ter de ser criados manualmente no Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="33e9b-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="33e9b-110">Se precisar de ajuda adicional, por favor abra um bilhete de apoio e especifique o âmbito do problema (incluindo o tipo de objeto que está a enviar) para que possamos ajudá-lo melhor.</span><span class="sxs-lookup"><span data-stu-id="33e9b-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>