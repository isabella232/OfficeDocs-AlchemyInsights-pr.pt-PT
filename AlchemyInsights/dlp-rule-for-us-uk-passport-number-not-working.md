---
title: Regra dLP para número de passaporte dos EUA/Reino Unido não funciona
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931273"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="e3b4d-102">Problemas com dlp - números de passaporte dos EUA/Reino Unido</span><span class="sxs-lookup"><span data-stu-id="e3b4d-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="e3b4d-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e3b4d-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e3b4d-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e3b4d-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e3b4d-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e3b4d-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e3b4d-109">**DLP emite problemas com números de passaporte dos EUA/Reino Unido**</span><span class="sxs-lookup"><span data-stu-id="e3b4d-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="e3b4d-110">Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** que não está a trabalhar para conteúdos que contenham um número de **passaporte EUA/Reino Unido** ao utilizar um tipo de informação sensível dLP em O365?</span><span class="sxs-lookup"><span data-stu-id="e3b4d-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e3b4d-111">Em caso afirmativo, certifique-se de que o seu conteúdo contém as informações necessárias para o que a política do DLP procura quando é avaliada.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="e3b4d-112">Por exemplo, para uma política de número de **passaporte dos EUA/Reino Unido** configurada com um nível de confiança de 75%, são avaliados e devem ser detetados para que a regra desencadeie</span><span class="sxs-lookup"><span data-stu-id="e3b4d-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="e3b4d-113">**[Formato:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nove dígitos</span><span class="sxs-lookup"><span data-stu-id="e3b4d-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="e3b4d-114">**[Padrão:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nove dígitos consecutivos</span><span class="sxs-lookup"><span data-stu-id="e3b4d-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="e3b4d-115">**[Chequeum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Não, não há Checksum.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="e3b4d-116">**[Definição:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Uma política de DLP está 75% confiante de que detetou este tipo de informação sensível se, dentro de uma proximidade de 300 caracteres:</span><span class="sxs-lookup"><span data-stu-id="e3b4d-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e3b4d-117">A função Func_usa_uk_passport encontra conteúdo que corresponda ao padrão.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="e3b4d-118">Uma palavra-chave de Keyword_passport é encontrada.</span><span class="sxs-lookup"><span data-stu-id="e3b4d-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="e3b4d-119">Por exemplo, a seguinte amostra seria desencadeada para a política de número de **passaporte dos EUA/Reino Unido:** Passaporte dos EUA número 123456789</span><span class="sxs-lookup"><span data-stu-id="e3b4d-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="e3b4d-120">Para obter mais informações sobre o que é necessário para que um número de passaporte dos EUA/Reino Unido seja detetado para o seu conteúdo, consulte a seguinte secção neste artigo: [O que os Tipos de Informação Sensível procuram para o Número de Passaporte supor EUA/Reino Unido](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="e3b4d-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="e3b4d-121">Utilizando um tipo de informação sensível incorporado diferente, consulte o seguinte artigo para obter informações sobre o que é necessário para outros tipos: O que os Tipos de [Informação Sensível procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e3b4d-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  