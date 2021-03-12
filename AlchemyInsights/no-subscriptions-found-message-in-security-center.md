---
title: Nenhuma subscrição encontrada mensagem no Centro de Segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713962"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="bcfbb-102">Nenhuma subscrição encontrada mensagem no Centro de Segurança</span><span class="sxs-lookup"><span data-stu-id="bcfbb-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="bcfbb-103">Se ao aceder ao Microsoft Defender Security Center obtém uma mensagem "Sem subscrições encontradas", significa que o Azure Ative Directory (AAD) utilizado para iniciar sessão no portal não tem uma licença ATP do Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="bcfbb-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="bcfbb-104">As licenças Windows E5 e Office E5 são licenças separadas.</span><span class="sxs-lookup"><span data-stu-id="bcfbb-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="bcfbb-105">Abra um caso de apoio se a licença foi comprada mas não for provisionada a este caso AAD.</span><span class="sxs-lookup"><span data-stu-id="bcfbb-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="bcfbb-106">Ou tem:</span><span class="sxs-lookup"><span data-stu-id="bcfbb-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="bcfbb-107">Um possível problema de provisionamento de licença.</span><span class="sxs-lookup"><span data-stu-id="bcfbb-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="bcfbb-108">Inadvertidamente, ademticou a licença a um Microsoft AAD diferente daquele utilizado para autenticação no serviço.</span><span class="sxs-lookup"><span data-stu-id="bcfbb-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>