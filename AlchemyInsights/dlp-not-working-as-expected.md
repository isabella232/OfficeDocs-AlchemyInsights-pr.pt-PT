---
title: DLP não funciona como esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932633"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="76c78-102">DLP não funciona como esperado</span><span class="sxs-lookup"><span data-stu-id="76c78-102">DLP not working as expected</span></span>

<span data-ttu-id="76c78-103">**Importante**: Muitos clientes SharePoint Online e OneDrive executam aplicações críticas ao negócio contra o serviço que executa em segundo plano.</span><span class="sxs-lookup"><span data-stu-id="76c78-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="76c78-104">Estes incluem migração de conteúdos, Prevenção de Perdas de Dados (DLP) e soluções de backup.</span><span class="sxs-lookup"><span data-stu-id="76c78-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="76c78-105">Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis e fiáveis para os seus utilizadores que dependem mais do serviço do que nunca em cenários de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="76c78-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="76c78-106">Em apoio a este objetivo, implementámos limites de estrangulamento mais apertados em aplicações de fundo (soluções de migração, DLP e backup) durante o dia da semana.</span><span class="sxs-lookup"><span data-stu-id="76c78-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="76c78-107">Deve esperar que estas aplicações atinjam uma entrada muito limitada durante estes tempos.</span><span class="sxs-lookup"><span data-stu-id="76c78-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="76c78-108">No entanto, durante as horas de noite e fim de semana para a região, o serviço estará pronto para processar um volume significativamente maior de pedidos de aplicações de fundo.</span><span class="sxs-lookup"><span data-stu-id="76c78-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="76c78-109">**Criação de DLP**</span><span class="sxs-lookup"><span data-stu-id="76c78-109">**Setting up DLP**</span></span>

<span data-ttu-id="76c78-110">Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** no Office 365 que não está a funcionar como esperado?</span><span class="sxs-lookup"><span data-stu-id="76c78-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="76c78-111">Em caso afirmativo, certifique-se de que a sua **política de DLP** está corretamente configurada e que os seus dados contêm o que a **política do DLP** procura quando está a ser avaliada.</span><span class="sxs-lookup"><span data-stu-id="76c78-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="76c78-112">As políticas de DLP permitem identificar e proteger informações sensíveis na sua organização.</span><span class="sxs-lookup"><span data-stu-id="76c78-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="76c78-113">Para configurar políticas de DLP, use a informação [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="76c78-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="76c78-114">**O que as políticas do DLP procuram**</span><span class="sxs-lookup"><span data-stu-id="76c78-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="76c78-115">Ao utilizar os **tipos de informação sensível incorporados** no Office 365 Security and Compliance center, as políticas de DLP procuram padrões e elementos específicos ao detetar estes tipos sensíveis.</span><span class="sxs-lookup"><span data-stu-id="76c78-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="76c78-116">**Tipos de informação sensível incorporados**</span><span class="sxs-lookup"><span data-stu-id="76c78-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="76c78-117">Para obter informações sobre os tipos sensíveis incorporados e o que uma política de DLP procura ao detetar o tipo Sensível, consulte: O que os [tipos de informação sensíveis procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="76c78-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="76c78-118">**Tipos de informação sensível personalizado**</span><span class="sxs-lookup"><span data-stu-id="76c78-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="76c78-119">Se estiver a tentar criar tipos de informação sensíveis personalizados, utilize o seguinte artigo para obter informações sobre como criar um tipo de [informação sensível personalizada: Criar um tipo](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)de informação sensível personalizado .</span><span class="sxs-lookup"><span data-stu-id="76c78-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="76c78-120">**Teste uma política de DLP**</span><span class="sxs-lookup"><span data-stu-id="76c78-120">**Test a DLP policy**</span></span>

<span data-ttu-id="76c78-121">Para testar os seus dados com um tipo de informação sensível incorporada ou personalizada, utilize a opção **do tipo Teste** em tipos de**informação sensíveis**de **classificações** > .</span><span class="sxs-lookup"><span data-stu-id="76c78-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="76c78-122">Para mais informações, consulte os tipos de [informação personalizadas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="76c78-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="76c78-123">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="76c78-123">**Reports**</span></span>
  
- <span data-ttu-id="76c78-124">Obtenha informações confidenciais de dados com [relatórios DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="76c78-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="76c78-125">Consulte detalhes específicos do evento com um Relatório de [Incidentes](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="76c78-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
