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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932454"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b7f11-102">DLP emite com números de cartão de crédito</span><span class="sxs-lookup"><span data-stu-id="b7f11-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="b7f11-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="b7f11-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b7f11-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="b7f11-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b7f11-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="b7f11-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b7f11-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="b7f11-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b7f11-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="b7f11-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b7f11-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="b7f11-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b7f11-109">**DLP emite com números de cartão de crédito**</span><span class="sxs-lookup"><span data-stu-id="b7f11-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="b7f11-110">Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um Número de **Cartão** de Crédito ao utilizar um tipo de informação sensível dLP em O365?</span><span class="sxs-lookup"><span data-stu-id="b7f11-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b7f11-111">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para desencadear a política dLP quando for avaliada.</span><span class="sxs-lookup"><span data-stu-id="b7f11-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b7f11-112">Por exemplo, para uma política de **Cartão** de Crédito configurada com um nível de confiança de 85%, são avaliados e devem ser detetados para que a regra desencadeie:</span><span class="sxs-lookup"><span data-stu-id="b7f11-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b7f11-113">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 dígitos que podem ser formatados ou não formatados (ddddddddddddddddddddddddddddd) e devem passar no teste Luhn.</span><span class="sxs-lookup"><span data-stu-id="b7f11-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b7f11-114">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Padrão muito complexo e robusto que deteta cartões de todas as grandes marcas em todo o mundo, incluindo Visa, MasterCard, Discover Card, JCB, American Express, cartões oferta e cartões de jantar.</span><span class="sxs-lookup"><span data-stu-id="b7f11-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b7f11-115">**[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Sim, o cheque Luhn.</span><span class="sxs-lookup"><span data-stu-id="b7f11-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b7f11-116">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Uma política de DLP está 85% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="b7f11-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b7f11-117">A função Func_credit_card encontra conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="b7f11-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b7f11-118">Um dos seguintes é verdade:</span><span class="sxs-lookup"><span data-stu-id="b7f11-118">One of the following is true:</span></span>

  - <span data-ttu-id="b7f11-119">Uma palavra-chave de Keyword_cc_verification é encontrada.</span><span class="sxs-lookup"><span data-stu-id="b7f11-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b7f11-120">Uma palavra-chave de Keyword_cc_name é encontrada</span><span class="sxs-lookup"><span data-stu-id="b7f11-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b7f11-121">A função Func_expiration_date encontra uma data no formato de data certa.</span><span class="sxs-lookup"><span data-stu-id="b7f11-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b7f11-122">O cheque passa</span><span class="sxs-lookup"><span data-stu-id="b7f11-122">The checksum passes</span></span>

    <span data-ttu-id="b7f11-123">Por exemplo, a seguinte amostra desencadearia uma Política de Números de Cartão de Crédito DLP:</span><span class="sxs-lookup"><span data-stu-id="b7f11-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b7f11-124">Visto: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="b7f11-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b7f11-125">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b7f11-125">Expires: 2/2009</span></span>

<span data-ttu-id="b7f11-126">Para obter mais informações sobre o que é necessário para que um Número de **Cartão** de Crédito seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram para cartão](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) de crédito#</span><span class="sxs-lookup"><span data-stu-id="b7f11-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b7f11-127">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b7f11-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  