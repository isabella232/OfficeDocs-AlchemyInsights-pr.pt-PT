---
title: Regra DLP para número de conta bancária dos EUA que não funciona
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679307"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="100b0-102">DLP emite com números de contas bancárias dos EUA</span><span class="sxs-lookup"><span data-stu-id="100b0-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="100b0-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="100b0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="100b0-104">**DLP emite com números de contas bancárias dos EUA**</span><span class="sxs-lookup"><span data-stu-id="100b0-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="100b0-105">Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** que não está a funcionar para conteúdos que contenham um **Número de Conta Bancária dos EUA** quando utilizar um tipo de informação sensível DLP em O365?</span><span class="sxs-lookup"><span data-stu-id="100b0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="100b0-106">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política de DLP procura quando é avaliada.</span><span class="sxs-lookup"><span data-stu-id="100b0-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="100b0-107">Por exemplo, para uma política **de número de conta bancária dos EUA** configurada com um nível de confiança de 85%, são avaliadas as seguintes e devem ser detetadas para que a regra desencadeie:</span><span class="sxs-lookup"><span data-stu-id="100b0-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="100b0-108">**[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 dígitos</span><span class="sxs-lookup"><span data-stu-id="100b0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="100b0-109">**[Padrão:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 dígitos consecutivos.</span><span class="sxs-lookup"><span data-stu-id="100b0-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="100b0-110">**[Checkum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Não, não há Cheques.</span><span class="sxs-lookup"><span data-stu-id="100b0-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="100b0-111">**[Definição:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Uma política de DLP está 75% confiante de que é detetado este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="100b0-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="100b0-112">A expressão regular Regex_usa_bank_account_number encontra conteúdo que corresponde ao padrão</span><span class="sxs-lookup"><span data-stu-id="100b0-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="100b0-113">Uma palavra-chave de Keyword_usa_Bank_Account é encontrada.</span><span class="sxs-lookup"><span data-stu-id="100b0-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="100b0-114">Por exemplo, a seguinte amostra desencadearia a política de **número de conta bancária dos EUA:** Conta 78344011</span><span class="sxs-lookup"><span data-stu-id="100b0-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="100b0-115">Para obter mais informações sobre o que é necessário para que um **Número de Conta Bancária dos EUA** seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de [Informação Sensível procuram para o Número de Conta Bancária dos EUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="100b0-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="100b0-116">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: [O que os Tipos de Informação Sensível procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="100b0-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  