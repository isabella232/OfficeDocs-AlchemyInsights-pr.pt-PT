---
title: Anti-paspam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821422"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="3ab28-102">Corrija os problemas de entrega de e-mail para código de erro 5.7.23</span><span class="sxs-lookup"><span data-stu-id="3ab28-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="3ab28-103">Verifique o registo de DNS SPF para o seu domínio num verificador de registo SPF ou DNS disponível publicamente na web.</span><span class="sxs-lookup"><span data-stu-id="3ab28-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="3ab28-104">Verifique se a mensagem de saída não foi identificada como spam pela Microsoft e encaminhada através do [Pool de Entrega de Alto Risco](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="3ab28-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="3ab28-105">As mensagens no Pool de Entrega de Alto Risco não passarão cheques SPF, pelo que não serão aceites pela organização de email de destino.</span><span class="sxs-lookup"><span data-stu-id="3ab28-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="3ab28-106">Se o problema persistir, poderá ter de contactar o administrador do anfitrião do correio para o qual está a tentar enviar e-mail.</span><span class="sxs-lookup"><span data-stu-id="3ab28-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="3ab28-107">Tome nota do erro externo detalhado disponível na mensagem de ressalto.</span><span class="sxs-lookup"><span data-stu-id="3ab28-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="3ab28-108">O suporte da Microsoft pode não ser capaz de ajudar mais.</span><span class="sxs-lookup"><span data-stu-id="3ab28-108">Microsoft support may not be able to assist further.</span></span>
