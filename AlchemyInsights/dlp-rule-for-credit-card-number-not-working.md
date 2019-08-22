---
title: Regra do DLP para número de cartão de crédito não funcionar
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529966"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="bfdfa-102">Problemas do DLP com números de cartão de crédito</span><span class="sxs-lookup"><span data-stu-id="bfdfa-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="bfdfa-103">Está a ter problemas com o **Data Loss Prevention (DLP)** não funcionar para o conteúdo que contenha um **Número de cartão de crédito** quando utilizar um tipo de informações sensíveis do DLP em O365?</span><span class="sxs-lookup"><span data-stu-id="bfdfa-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="bfdfa-104">Se assim for, certifique-se de conteúdo contém as informações necessárias para activar a política DLP quando é avaliado.</span><span class="sxs-lookup"><span data-stu-id="bfdfa-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="bfdfa-105">Por exemplo, para uma **política de cartão de crédito** configurado com um nível de confiança de 85%, a seguir é avaliados e deve ser detectada para a regra accionar:</span><span class="sxs-lookup"><span data-stu-id="bfdfa-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="bfdfa-106">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou formatada (dddddddddddddddd) e tem de passar no teste de Luhn.</span><span class="sxs-lookup"><span data-stu-id="bfdfa-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="bfdfa-107">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Padrão de muito complexo e robusto que detecta placas de todas as marcas principais em todo o mundo, incluindo Visa, MasterCard, descobrir o cartão, JCB, American Express, cartões de oferta e cartões de diner.</span><span class="sxs-lookup"><span data-stu-id="bfdfa-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="bfdfa-108">**[Soma de verificação:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, a soma de verificação de Luhn</span><span class="sxs-lookup"><span data-stu-id="bfdfa-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="bfdfa-109">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política DLP é de 85% de certeza de que detectou este tipo de informações sensíveis se, num raio de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="bfdfa-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="bfdfa-110">A função Func_credit_card localiza conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="bfdfa-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="bfdfa-111">Uma das seguintes afirmações é verdadeira:</span><span class="sxs-lookup"><span data-stu-id="bfdfa-111">One of the following is true:</span></span>

  - <span data-ttu-id="bfdfa-112">Foi encontrada uma palavra-chave de Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="bfdfa-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="bfdfa-113">Encontra-se uma palavra-chave de Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="bfdfa-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="bfdfa-114">A função Func_expiration_date localiza uma data no formato de data à direita.</span><span class="sxs-lookup"><span data-stu-id="bfdfa-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="bfdfa-115">As fases de soma de verificação</span><span class="sxs-lookup"><span data-stu-id="bfdfa-115">The checksum passes</span></span>

    <span data-ttu-id="bfdfa-116">Por exemplo, o seguinte exemplo daria origem para uma política de número de cartão de crédito do DLP:</span><span class="sxs-lookup"><span data-stu-id="bfdfa-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="bfdfa-117">Visto: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="bfdfa-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="bfdfa-118">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="bfdfa-118">Expires: 2/2009</span></span>

<span data-ttu-id="bfdfa-119">Para mais informações sobre o que é necessário para um **Número de cartão de crédito** a ser detectado para o seu conteúdo, consulte a secção seguinte deste artigo: [O que o sensíveis a maiúsculas e tipos de informação procure cartão de crédito #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="bfdfa-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="bfdfa-120">Utilizando um tipo de informações sensíveis incorporados diferentes, consulte o artigo seguinte para obter informações sobre o que é necessário para outros tipos: [Procurar o que o sensíveis a maiúsculas e tipos de informação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="bfdfa-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  