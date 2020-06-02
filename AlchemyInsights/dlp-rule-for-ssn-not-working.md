---
title: Regra do DLP para a SSN não funcionar
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507381"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d64b6-102">Problemas de DLP com números de Segurança Social</span><span class="sxs-lookup"><span data-stu-id="d64b6-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d64b6-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="d64b6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d64b6-104">**Problemas de DLP com SSNs**</span><span class="sxs-lookup"><span data-stu-id="d64b6-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="d64b6-105">Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a trabalhar para conteúdos que contenham um **Número de Segurança Social (SSN)** quando utiliza um tipo de informação sensível na Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="d64b6-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="d64b6-106">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP está a procurar.</span><span class="sxs-lookup"><span data-stu-id="d64b6-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d64b6-107">Por exemplo, para uma política da SSN configurada com um nível de confiança de 85%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie:</span><span class="sxs-lookup"><span data-stu-id="d64b6-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d64b6-108">**[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 dígitos, que podem estar num padrão formatado ou não equipado</span><span class="sxs-lookup"><span data-stu-id="d64b6-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d64b6-109">**[Padrão:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatro funções procuram SSNs em quatro padrões diferentes:</span><span class="sxs-lookup"><span data-stu-id="d64b6-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d64b6-110">Func_ssn encontra SSNs com formatação forte pré-2011 que são formatadas com traços ou espaços (ddd-ddd-dddd OU ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="d64b6-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d64b6-111">Func_unformatted_ssn encontra SSNs com formatação forte pré-2011 que não são formatadas como nove dígitos consecutivos (dddddddd)</span><span class="sxs-lookup"><span data-stu-id="d64b6-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d64b6-112">Func_randomized_formatted_ssn encontra SSNs pós-2011 que são formatadas com traços ou espaços (ddd-ddd-dddd OR ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="d64b6-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d64b6-113">Func_randomized_unformatted_ssn encontra SSNs pós-2011 que não são formatadas como nove dígitos consecutivos (ddddddd)</span><span class="sxs-lookup"><span data-stu-id="d64b6-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d64b6-114">**[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Não, não há Cheques.</span><span class="sxs-lookup"><span data-stu-id="d64b6-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d64b6-115">**[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Uma política de DLP está 85% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="d64b6-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d64b6-116">A [função Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) encontra conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="d64b6-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d64b6-117">Uma palavra-chave de [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) é encontrada.</span><span class="sxs-lookup"><span data-stu-id="d64b6-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="d64b6-118">Exemplos de palavras-chave incluem: *Segurança Social, Segurança Social#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="d64b6-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d64b6-119">Por exemplo, a seguinte amostra desencadearia para a política DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d64b6-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d64b6-120">Para obter mais informações sobre o que é necessário para que as SSNs sejam detetadas para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram por SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d64b6-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d64b6-121">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d64b6-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  