---
title: Resolução de problemas da ponta de segurança para verificação de deteção de fraudes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504994"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="bd6d8-102">Resolução de problemas da ponta de segurança para verificação de deteção de fraudes</span><span class="sxs-lookup"><span data-stu-id="bd6d8-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="bd6d8-103">Se estiver a receber uma dica de segurança que diz "O remetente falhou nas nossas verificações de deteção de fraudes e pode não ser quem parece ser", então o remetente não passou nem verificações de autenticação DKIM ou SPF.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="bd6d8-104">O melhor método para resolver isto é o remetente autorizar-se a si próprio.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="bd6d8-105">Se o remetente estiver a enviar em seu nome, tem de os autorizar adicionando o endereço IP do remetente ao seu registo SPF.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="bd6d8-106">Consulte [a resolução de problemas da ponta de segurança vermelha (suspeita) para verificação de fraudes](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="bd6d8-107">Aqui estão outros links que podem ajudar:</span><span class="sxs-lookup"><span data-stu-id="bd6d8-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="bd6d8-108">Como a Microsoft usa o quadro de política de remetente (SPF) para evitar falsificações</span><span class="sxs-lookup"><span data-stu-id="bd6d8-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="bd6d8-109">Criar SPF para ajudar a prevenir a falsificação</span><span class="sxs-lookup"><span data-stu-id="bd6d8-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
