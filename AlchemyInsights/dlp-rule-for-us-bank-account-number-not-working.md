---
title: Regra do DLP para número de conta bancária dos EUA não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932560"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="3008d-102">DLP emite com números de conta bancária dos EUA</span><span class="sxs-lookup"><span data-stu-id="3008d-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="3008d-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="3008d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3008d-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="3008d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3008d-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="3008d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3008d-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="3008d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3008d-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="3008d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3008d-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="3008d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3008d-109">**DLP emite com números de conta bancária dos EUA**</span><span class="sxs-lookup"><span data-stu-id="3008d-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="3008d-110">Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um **Número de Conta Bancária dos EUA** ao utilizar um tipo de informação sensível dLP em O365?</span><span class="sxs-lookup"><span data-stu-id="3008d-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3008d-111">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP procura quando é avaliada.</span><span class="sxs-lookup"><span data-stu-id="3008d-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="3008d-112">Por exemplo, para uma política de número de **conta bancária dos EUA** configurada com um nível de confiança de 85%, são avaliados e devem ser detetados para que a regra desencadeie:</span><span class="sxs-lookup"><span data-stu-id="3008d-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3008d-113">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 dígitos</span><span class="sxs-lookup"><span data-stu-id="3008d-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="3008d-114">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 dígitos consecutivos.</span><span class="sxs-lookup"><span data-stu-id="3008d-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="3008d-115">**[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há Checksum.</span><span class="sxs-lookup"><span data-stu-id="3008d-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="3008d-116">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Uma política de DLP está 75% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="3008d-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3008d-117">A expressão regular Regex_usa_bank_account_number encontra conteúdo que corresponda ao padrão</span><span class="sxs-lookup"><span data-stu-id="3008d-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="3008d-118">Uma palavra-chave de Keyword_usa_Bank_Account é encontrada.</span><span class="sxs-lookup"><span data-stu-id="3008d-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="3008d-119">Por exemplo, a seguinte amostra seria desencadeada para a política do número de **conta bancária dos EUA:** Conta de verificação 78344011</span><span class="sxs-lookup"><span data-stu-id="3008d-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="3008d-120">Para obter mais informações sobre o que é necessário para que um Número de **Conta Bancária dos EUA** seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: O que os Tipos de [Informação Sensível procuram para](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number) o Número de Conta Bancária dos EUA</span><span class="sxs-lookup"><span data-stu-id="3008d-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="3008d-121">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3008d-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  