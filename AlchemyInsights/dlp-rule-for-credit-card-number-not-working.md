---
title: Regra do DLP para número de cartão de crédito não funcionar
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919091"
---
<span data-ttu-id="08402-p101">Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contenha um **Número de cartão de crédito** quando utilizar um tipo de informações sensíveis do DLP em O365? Se assim for, certifique-se de conteúdo contém as informações necessárias para activar a política DLP quando é avaliado. Por exemplo, para uma **política de cartão de crédito** configurado com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar:</span><span class="sxs-lookup"><span data-stu-id="08402-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="08402-105">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou formatada (dddddddddddddddd) e tem de passar no teste de Luhn.</span><span class="sxs-lookup"><span data-stu-id="08402-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="08402-106">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Padrão de muito complexo e robusto que detecta placas de todas as marcas principais em todo o mundo, incluindo Visa, Mastercard, descobrir o cartão, JCB, American Express, cartões de oferta e cartões de diner.</span><span class="sxs-lookup"><span data-stu-id="08402-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="08402-107">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação de Luhn</span><span class="sxs-lookup"><span data-stu-id="08402-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="08402-108">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política DLP é de 85% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="08402-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="08402-109">A função Func_credit_card localiza conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="08402-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="08402-110">Uma das seguintes afirmações é verdadeira:</span><span class="sxs-lookup"><span data-stu-id="08402-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="08402-111">Foi encontrada uma palavra-chave de Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="08402-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="08402-112">Encontra-se uma palavra-chave de Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="08402-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="08402-113">A função Func_expiration_date localiza uma data no formato de data à direita.</span><span class="sxs-lookup"><span data-stu-id="08402-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="08402-114">As fases de soma de verificação</span><span class="sxs-lookup"><span data-stu-id="08402-114">The checksum passes</span></span>
    
    <span data-ttu-id="08402-115">Por exemplo, o seguinte exemplo daria origem para uma política de número de cartão de crédito do DLP:</span><span class="sxs-lookup"><span data-stu-id="08402-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="08402-116">Visto: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="08402-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="08402-117">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="08402-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="08402-118">Para mais informações sobre o que é necessário para um **Número de cartão de crédito** a ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="08402-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="08402-119">Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="08402-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

