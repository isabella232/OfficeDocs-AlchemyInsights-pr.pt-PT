---
title: Nenhuma mensagem de subscrições encontrada no Centro de Segurança
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544119"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="ac911-102">Nenhuma mensagem de subscrições encontrada no Centro de Segurança</span><span class="sxs-lookup"><span data-stu-id="ac911-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="ac911-103">Se ao aceder ao Centro de Segurança do Microsoft Defender receber a mensagem "Não foram encontradas subscrições", significa que o Azure Active Directory (AAD) utilizado para loginar o utilizador no portal não tem uma licença Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="ac911-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="ac911-104">Os Windows E5 e Office E5 são licenças separadas.</span><span class="sxs-lookup"><span data-stu-id="ac911-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="ac911-105">Abra um caso de suporte se a licença tiver sido comprada, mas não tiver sido aprovisionada para esta instância do AAD.</span><span class="sxs-lookup"><span data-stu-id="ac911-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="ac911-106">Tem:</span><span class="sxs-lookup"><span data-stu-id="ac911-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="ac911-107">Um possível problema de aprovisionamento de licenças.</span><span class="sxs-lookup"><span data-stu-id="ac911-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="ac911-108">Aprovisionou inadvertidamente a licença para um Microsoft AAD diferente da que foi utilizada para a autenticação no serviço.</span><span class="sxs-lookup"><span data-stu-id="ac911-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>