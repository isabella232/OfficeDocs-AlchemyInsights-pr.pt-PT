---
title: Regra DLP para número de cartão de crédito que não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507417"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="55dfc-102">Problemas de DLP com números de cartão de crédito</span><span class="sxs-lookup"><span data-stu-id="55dfc-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="55dfc-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="55dfc-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="55dfc-104">**Problemas de DLP com números de cartão de crédito**</span><span class="sxs-lookup"><span data-stu-id="55dfc-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="55dfc-105">Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a funcionar para conteúdos que contenham um **Número de Cartão de Crédito** quando utilizar um tipo de informação sensível DLP em O365?</span><span class="sxs-lookup"><span data-stu-id="55dfc-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="55dfc-106">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para desencadear a política DLP quando esta for avaliada.</span><span class="sxs-lookup"><span data-stu-id="55dfc-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="55dfc-107">Por exemplo, para uma **política de cartão** de crédito configurada com um nível de confiança de 85%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie:</span><span class="sxs-lookup"><span data-stu-id="55dfc-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="55dfc-108">**[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 dígitos que podem ser formatados ou não equipados (ddddddddddddddddddddd) e devem passar no teste luhn.</span><span class="sxs-lookup"><span data-stu-id="55dfc-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="55dfc-109">**[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Um padrão muito complexo e robusto que deteta cartões de todas as grandes marcas em todo o mundo, incluindo Visa, MasterCard, Discover Card, JCB, American Express, cartões oferta e cartões de jantar.</span><span class="sxs-lookup"><span data-stu-id="55dfc-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="55dfc-110">**[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Sim, o cheque luhn</span><span class="sxs-lookup"><span data-stu-id="55dfc-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="55dfc-111">**[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Uma política de DLP está 85% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="55dfc-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="55dfc-112">A função Func_credit_card encontra conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="55dfc-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="55dfc-113">Um dos seguintes é verdade:</span><span class="sxs-lookup"><span data-stu-id="55dfc-113">One of the following is true:</span></span>

  - <span data-ttu-id="55dfc-114">Uma palavra-chave de Keyword_cc_verification é encontrada.</span><span class="sxs-lookup"><span data-stu-id="55dfc-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="55dfc-115">Uma palavra-chave de Keyword_cc_name é encontrada</span><span class="sxs-lookup"><span data-stu-id="55dfc-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="55dfc-116">A função Func_expiration_date encontra uma data no formato de data certa.</span><span class="sxs-lookup"><span data-stu-id="55dfc-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="55dfc-117">A parte de verificação passa</span><span class="sxs-lookup"><span data-stu-id="55dfc-117">The checksum passes</span></span>

    <span data-ttu-id="55dfc-118">Por exemplo, a seguinte amostra desencadearia uma Política de Números de Cartão de Crédito DLP:</span><span class="sxs-lookup"><span data-stu-id="55dfc-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="55dfc-119">Visto: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="55dfc-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="55dfc-120">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="55dfc-120">Expires: 2/2009</span></span>

<span data-ttu-id="55dfc-121">Para obter mais informações sobre o que é necessário para que um **Número de Cartão** de Crédito seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram por Cartão de Crédito#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="55dfc-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="55dfc-122">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="55dfc-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  