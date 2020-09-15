---
title: Regra DLP para número de passaporte dos EUA/Reino Unido que não funcione
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679235"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="f6be9-102">Problemas com números de passaportes DLP - EUA/Reino Unido</span><span class="sxs-lookup"><span data-stu-id="f6be9-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="f6be9-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="f6be9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f6be9-104">**Problemas de DLP com números de passaportes EUA/Reino Unido**</span><span class="sxs-lookup"><span data-stu-id="f6be9-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="f6be9-105">Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a trabalhar para conteúdos que contenham um **número de passaporte dos EUA/Reino Unido** quando utilizar um tipo de informação sensível DLP em O365?</span><span class="sxs-lookup"><span data-stu-id="f6be9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f6be9-106">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política de DLP procura quando é avaliada.</span><span class="sxs-lookup"><span data-stu-id="f6be9-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="f6be9-107">Por exemplo, para uma política **de número de passaportes dos EUA/Reino Unido** configurada com um nível de confiança de 75%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie</span><span class="sxs-lookup"><span data-stu-id="f6be9-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="f6be9-108">**[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nove dígitos</span><span class="sxs-lookup"><span data-stu-id="f6be9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="f6be9-109">**[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nove dígitos consecutivos</span><span class="sxs-lookup"><span data-stu-id="f6be9-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="f6be9-110">**[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há Cheques.</span><span class="sxs-lookup"><span data-stu-id="f6be9-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="f6be9-111">**[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Uma política de DLP está 75% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="f6be9-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f6be9-112">A função Func_usa_uk_passport encontra conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="f6be9-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f6be9-113">Uma palavra-chave de Keyword_passport é encontrada.</span><span class="sxs-lookup"><span data-stu-id="f6be9-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="f6be9-114">Por exemplo, a seguinte amostra desencadearia a política de **número de passaportes dos EUA/Reino Unido:** Número de passaporte dos EUA 123456789</span><span class="sxs-lookup"><span data-stu-id="f6be9-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="f6be9-115">Para obter mais informações sobre o que é necessário para que um número de passaporte dos EUA/Reino Unido seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os tipos de informação sensível procuram para o número de passaporte dos EUA/Reino Unido](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="f6be9-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="f6be9-116">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f6be9-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  