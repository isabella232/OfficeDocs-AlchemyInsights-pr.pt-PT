---
title: A sugestão de segurança para detecção de fraudes de resolução de problemas verifica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533209"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="be63b-102">A sugestão de segurança para detecção de fraudes de resolução de problemas verifica</span><span class="sxs-lookup"><span data-stu-id="be63b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="be63b-103">Se estiver a obter uma sugestão de segurança que indica "o remetente falhou o nosso controlos de detecção de fraudes e poderá não ser que o que parecem estar", em seguida, o remetente falhou a transmissão de DKIM ou SPF verificações de autenticação.</span><span class="sxs-lookup"><span data-stu-id="be63b-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="be63b-104">É o melhor método para resolver este problema para o remetente autorizar próprios.</span><span class="sxs-lookup"><span data-stu-id="be63b-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="be63b-105">Se o remetente está a enviar em seu nome, terá de lhes confira adicionando o endereço IP do remetente ao registo SPF.</span><span class="sxs-lookup"><span data-stu-id="be63b-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="be63b-106">Para obter mais informações, consulte [a sugestão de segurança (suspeitas) vermelho para detecção de fraudes de resolução de problemas verifica](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="be63b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="be63b-107">Eis algumas hiperligações que podem ajudar:</span><span class="sxs-lookup"><span data-stu-id="be63b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="be63b-108">Como o Office 365 utiliza o quadro de política de emissor (SPF) para impedir a fraude de identidade</span><span class="sxs-lookup"><span data-stu-id="be63b-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="be63b-109">Configurar SPF no Office 365 para ajudar a impedir o spoofing</span><span class="sxs-lookup"><span data-stu-id="be63b-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
