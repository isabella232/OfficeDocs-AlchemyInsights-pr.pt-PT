---
title: DLP não funciona como esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507489"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="42b2d-102">DLP não funciona como esperado</span><span class="sxs-lookup"><span data-stu-id="42b2d-102">DLP not working as expected</span></span>

<span data-ttu-id="42b2d-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="42b2d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="42b2d-104">**Criação de DLP**</span><span class="sxs-lookup"><span data-stu-id="42b2d-104">**Setting up DLP**</span></span>

<span data-ttu-id="42b2d-105">Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** no Office 365 que não funciona como esperado?</span><span class="sxs-lookup"><span data-stu-id="42b2d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="42b2d-106">Em caso afirmativo, certifique-se de que a sua **política DLP** está corretamente configurada e que os seus dados contêm o que a **política de DLP** procura quando está a ser avaliada.</span><span class="sxs-lookup"><span data-stu-id="42b2d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="42b2d-107">As políticas de DLP permitem identificar e proteger informações sensíveis na sua organização.</span><span class="sxs-lookup"><span data-stu-id="42b2d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="42b2d-108">Para configurar as políticas DLP, utilize a informação [aqui.](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)</span><span class="sxs-lookup"><span data-stu-id="42b2d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="42b2d-109">**O que as políticas de DLP procuram**</span><span class="sxs-lookup"><span data-stu-id="42b2d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="42b2d-110">Ao utilizar os **tipos de informação sensível incorporados** nos centros de Segurança e Conformidade, as políticas DLP procuram padrões e elementos específicos ao detetar estes tipos sensíveis.</span><span class="sxs-lookup"><span data-stu-id="42b2d-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="42b2d-111">**Tipos de informação sensível incorporados**</span><span class="sxs-lookup"><span data-stu-id="42b2d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="42b2d-112">Para obter informações sobre os tipos sensíveis incorporados e sobre o que uma política DLP procura ao detetar o tipo Sensível, consulte: [O que os tipos de informação sensíveis procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="42b2d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="42b2d-113">**Tipos de informação sensível personalizados**</span><span class="sxs-lookup"><span data-stu-id="42b2d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="42b2d-114">Se estiver a tentar criar tipos de informação sensíveis personalizados, utilize o seguinte artigo para obter informações sobre como criar um tipo de informação sensível personalizado: [Criar um tipo de informação sensível personalizado](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="42b2d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="42b2d-115">**Testar uma política de DLP**</span><span class="sxs-lookup"><span data-stu-id="42b2d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="42b2d-116">Para testar os seus dados com um tipo de informação sensível incorporada ou personalizada, utilize a opção **tipo teste** em **classificações**  >  **Tipos de informação sensíveis**.</span><span class="sxs-lookup"><span data-stu-id="42b2d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="42b2d-117">Para obter mais informações, consulte [test tipos de informações sensíveis personalizadas.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="42b2d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="42b2d-118">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="42b2d-118">**Reports**</span></span>
  
- <span data-ttu-id="42b2d-119">Obtenha informações confidenciais de dados com [relatórios DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="42b2d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="42b2d-120">Consulte detalhes específicos do evento com um [Relatório de Incidentes.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="42b2d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
