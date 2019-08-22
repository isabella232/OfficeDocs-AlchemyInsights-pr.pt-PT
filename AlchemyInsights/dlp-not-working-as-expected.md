---
title: DLP não funcionar conforme esperado
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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530301"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e4dad-102">DLP não funcionar conforme esperado</span><span class="sxs-lookup"><span data-stu-id="e4dad-102">DLP not working as expected</span></span>

<span data-ttu-id="e4dad-103">Está a ter problemas com o **Data Loss Prevention (DLP)** no Office 365 não funcionar conforme esperado?</span><span class="sxs-lookup"><span data-stu-id="e4dad-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e4dad-104">Se assim for, certifique-se de que a **política do DLP** está configurado correctamente e que os seus dados contiverem que a **política do DLP** está à procura quando este está a ser avaliada.</span><span class="sxs-lookup"><span data-stu-id="e4dad-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="e4dad-105">**Configurar DLP**</span><span class="sxs-lookup"><span data-stu-id="e4dad-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="e4dad-106">Políticas do DLP permite-lhe identificar e proteger informações confidenciais na sua organização.</span><span class="sxs-lookup"><span data-stu-id="e4dad-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e4dad-107">Para configurar as políticas do DLP, utilize as informações [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="e4dad-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e4dad-108">**O que procuram políticas DLP**</span><span class="sxs-lookup"><span data-stu-id="e4dad-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e4dad-109">Quando utilizar os **tipos de informações sensíveis incorporada** no Centro de segurança do Office 365 e conformidade, as políticas do DLP procuram padrões específicos e elementos quando detectar estes tipos sensíveis.</span><span class="sxs-lookup"><span data-stu-id="e4dad-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e4dad-110">**Tipos de informações sensíveis incorporada**</span><span class="sxs-lookup"><span data-stu-id="e4dad-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e4dad-111">Para obter informações sobre os tipos de sensíveis incorporados e o que uma política do DLP procura quando detectar o tipo sensível, consulte: [procuram a que os tipos de informações sensíveis](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="e4dad-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="e4dad-112">**Tipos de informações sensíveis personalizadas**</span><span class="sxs-lookup"><span data-stu-id="e4dad-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e4dad-113">Se está a tentar criar tipos de informações sensíveis personalizadas, utilize o seguinte artigo para obter informações sobre como criar um tipo personalizado sensível: [criar um tipo de informações sensíveis personalizadas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="e4dad-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e4dad-114">**Teste uma política do DLP**</span><span class="sxs-lookup"><span data-stu-id="e4dad-114">**Test a DLP policy**</span></span>

<span data-ttu-id="e4dad-115">Para testar os seus dados com um tipo de informações sensíveis incorporados ou personalizados, utilize a opção de **tipo de teste** em **classificações** > **tipos de informações sensíveis**.</span><span class="sxs-lookup"><span data-stu-id="e4dad-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e4dad-116">Para mais informações, consulte [tipos de informações sensíveis personalizadas de ensaio](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="e4dad-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e4dad-117">**Relatórios**</span><span class="sxs-lookup"><span data-stu-id="e4dad-117">**Reports**</span></span>
  
- <span data-ttu-id="e4dad-118">Obter conhecimentos aprofundados de dados importantes com [relatórios do DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e4dad-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e4dad-119">Ver detalhes do evento com um [Relatório de acidente](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="e4dad-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
