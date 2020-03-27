---
title: Regra dLP para número de cartão de crédito não funcionando
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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977209"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="3924b-102">DLP emite com números de cartão de crédito</span><span class="sxs-lookup"><span data-stu-id="3924b-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="3924b-103">**Importante**: Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis – Visite os Ajustes de [FuncionalidadeS Temporárias Online SharePoint](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="3924b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="3924b-104">**DLP emite com números de cartão de crédito**</span><span class="sxs-lookup"><span data-stu-id="3924b-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="3924b-105">Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um Número de **Cartão** de Crédito ao utilizar um tipo de informação sensível dLP em O365?</span><span class="sxs-lookup"><span data-stu-id="3924b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3924b-106">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para desencadear a política dLP quando for avaliada.</span><span class="sxs-lookup"><span data-stu-id="3924b-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="3924b-107">Por exemplo, para uma política de **Cartão** de Crédito configurada com um nível de confiança de 85%, são avaliados e devem ser detetados para que a regra desencadeie:</span><span class="sxs-lookup"><span data-stu-id="3924b-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3924b-108">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatados (ddddddddddddddddddddddddddddd) e devem passar no teste Luhn.</span><span class="sxs-lookup"><span data-stu-id="3924b-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="3924b-109">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Padrão muito complexo e robusto que deteta cartões de todas as grandes marcas em todo o mundo, incluindo Visa, MasterCard, Discover Card, JCB, American Express, cartões oferta e cartões de jantar.</span><span class="sxs-lookup"><span data-stu-id="3924b-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="3924b-110">**[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, o cheque Luhn.</span><span class="sxs-lookup"><span data-stu-id="3924b-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="3924b-111">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política de DLP está 85% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="3924b-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3924b-112">A função Func_credit_card encontra conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="3924b-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3924b-113">Um dos seguintes é verdade:</span><span class="sxs-lookup"><span data-stu-id="3924b-113">One of the following is true:</span></span>

  - <span data-ttu-id="3924b-114">Uma palavra-chave de Keyword_cc_verification é encontrada.</span><span class="sxs-lookup"><span data-stu-id="3924b-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="3924b-115">Uma palavra-chave de Keyword_cc_name é encontrada</span><span class="sxs-lookup"><span data-stu-id="3924b-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="3924b-116">A função Func_expiration_date encontra uma data no formato de data certa.</span><span class="sxs-lookup"><span data-stu-id="3924b-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="3924b-117">O cheque passa</span><span class="sxs-lookup"><span data-stu-id="3924b-117">The checksum passes</span></span>

    <span data-ttu-id="3924b-118">Por exemplo, a seguinte amostra desencadearia uma Política de Números de Cartão de Crédito DLP:</span><span class="sxs-lookup"><span data-stu-id="3924b-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="3924b-119">Visto: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="3924b-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="3924b-120">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="3924b-120">Expires: 2/2009</span></span>

<span data-ttu-id="3924b-121">Para obter mais informações sobre o que é necessário para que um Número de **Cartão** de Crédito seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram para cartão](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) de crédito#</span><span class="sxs-lookup"><span data-stu-id="3924b-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="3924b-122">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3924b-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  