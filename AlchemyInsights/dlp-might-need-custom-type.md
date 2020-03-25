---
title: DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932669"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="5559c-102">DLP pode precisar de um tipo personalizado</span><span class="sxs-lookup"><span data-stu-id="5559c-102">DLP might need a custom type</span></span>

<span data-ttu-id="5559c-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="5559c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5559c-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="5559c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5559c-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="5559c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5559c-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="5559c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5559c-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="5559c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5559c-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="5559c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5559c-109">**DLP pode requerer um tipo de informação personalizada**</span><span class="sxs-lookup"><span data-stu-id="5559c-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="5559c-110">Com uma política de prevenção de perdas de dados (DLP), pode identificar e proteger dados sensíveis na sua organização.</span><span class="sxs-lookup"><span data-stu-id="5559c-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="5559c-111">Em alguns cenários, poderá ser necessário criar o seu **próprio** tipo de informação personalizada e sensível para proteger os dados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="5559c-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="5559c-112">Por exemplo, a sua organização pode precisar de identificar e proteger iDs ou outros dados de funcionários em algum formato específico do seu org. Em caso afirmativo, consulte os seguintes artigos para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="5559c-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="5559c-113">**Personalize um tipo de informação sensível incorporada**</span><span class="sxs-lookup"><span data-stu-id="5559c-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="5559c-114">Se um tipo de informação sensível incorporado atender às suas necessidades com apenas alguns ajustes, pode [personalizar um tipo de informação sensível incorporado](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5559c-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="5559c-115">Por exemplo, pode adicionar ou remover palavras-chave, ou adicionar ou remover provas de apoio, como uma data ou endereço.</span><span class="sxs-lookup"><span data-stu-id="5559c-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="5559c-116">**Criar um tipo de informação sensível personalizado**</span><span class="sxs-lookup"><span data-stu-id="5559c-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="5559c-117">Mas se precisar de identificar e proteger completamente um tipo diferente de informação sensível, pode criar um tipo de [informação sensível personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) na UI do Centro de Conformidade & Segurança.</span><span class="sxs-lookup"><span data-stu-id="5559c-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="5559c-118">**Criar um tipo de informação sensível personalizado em Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="5559c-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="5559c-119">Finalmente, se o UI não fornecer todas as opções de que necessita, pode criar um tipo de [informação sensível personalizado em Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="5559c-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="5559c-120">Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5559c-120">By starting with an XML file, you can use every option available.</span></span>
