---
title: Resolução de problemas de autenticação SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826426"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="6ba0b-102">Resolução de problemas de autenticação SMTP</span><span class="sxs-lookup"><span data-stu-id="6ba0b-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="6ba0b-103">Se estiver a obter erros 5.7.57 ou 5.7.3 ao tentar enviar e-mail SMTP e autenticar com um cliente ou aplicação, há algumas coisas que deve verificar:</span><span class="sxs-lookup"><span data-stu-id="6ba0b-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="6ba0b-104">A submissão autenticada do SMTP pode ser desativada no seu inquilino ou na caixa de correio que está a tentar utilizar (verifique ambas as definições).</span><span class="sxs-lookup"><span data-stu-id="6ba0b-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="6ba0b-105">Para ler mais, consulte [Ativar ou desativar a submissão do cliente autenticado SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="6ba0b-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="6ba0b-106">Verifique se [os Incumprimentos de Segurança Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) estão ativados para o seu inquilino; se ativado, a autenticação SMTP utilizando a autenticação básica (também conhecida como legado; isto utilizará o nome de utilizador e a palavra-passe) falhará.</span><span class="sxs-lookup"><span data-stu-id="6ba0b-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
