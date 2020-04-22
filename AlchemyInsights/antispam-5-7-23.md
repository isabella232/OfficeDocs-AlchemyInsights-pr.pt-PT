---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676508"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="22471-102">Corrija os problemas de entrega de e-mail para código de erro 5.7.23</span><span class="sxs-lookup"><span data-stu-id="22471-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="22471-103">Verifique o registo DoNs SPF para o seu domínio num verificador de registoS SPF ou DNS publicamente disponível na web.</span><span class="sxs-lookup"><span data-stu-id="22471-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="22471-104">Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do Pool de Entrega de [Alto Risco](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="22471-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="22471-105">As mensagens no Pool de Entrega de Alto Risco não passarão em cheques SPF, pelo que não serão aceites pela organização de e-mails de destino.</span><span class="sxs-lookup"><span data-stu-id="22471-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="22471-106">Se o problema persistir, poderá ter de contactar o administrador do correio para o qual está a tentar enviar e-mail.</span><span class="sxs-lookup"><span data-stu-id="22471-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="22471-107">Tome nota do erro externo detalhado disponível na mensagem de ressalta.</span><span class="sxs-lookup"><span data-stu-id="22471-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="22471-108">O suporte da Microsoft pode não ser capaz de ajudar mais.</span><span class="sxs-lookup"><span data-stu-id="22471-108">Microsoft support may not be able to assist further.</span></span>
