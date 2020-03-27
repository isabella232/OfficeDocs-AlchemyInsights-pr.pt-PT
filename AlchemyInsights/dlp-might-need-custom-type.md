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
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977281"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="18d36-102">DLP pode precisar de um tipo personalizado</span><span class="sxs-lookup"><span data-stu-id="18d36-102">DLP might need a custom type</span></span>

<span data-ttu-id="18d36-103">**Importante**: Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis – Visite os Ajustes de [FuncionalidadeS Temporárias Online SharePoint](https://aka.ms/ODSPAdjustments) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="18d36-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="18d36-104">**DLP pode requerer um tipo de informação personalizada**</span><span class="sxs-lookup"><span data-stu-id="18d36-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="18d36-105">Com uma política de prevenção de perdas de dados (DLP), pode identificar e proteger dados sensíveis na sua organização.</span><span class="sxs-lookup"><span data-stu-id="18d36-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="18d36-106">Em alguns cenários, poderá ser necessário criar o seu **próprio** tipo de informação personalizada e sensível para proteger os dados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="18d36-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="18d36-107">Por exemplo, a sua organização pode precisar de identificar e proteger iDs ou outros dados de funcionários em algum formato específico do seu org. Em caso afirmativo, consulte os seguintes artigos para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="18d36-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="18d36-108">**Personalize um tipo de informação sensível incorporada**</span><span class="sxs-lookup"><span data-stu-id="18d36-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="18d36-109">Se um tipo de informação sensível incorporado atender às suas necessidades com apenas alguns ajustes, pode [personalizar um tipo de informação sensível incorporado](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="18d36-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="18d36-110">Por exemplo, pode adicionar ou remover palavras-chave, ou adicionar ou remover provas de apoio, como uma data ou endereço.</span><span class="sxs-lookup"><span data-stu-id="18d36-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="18d36-111">**Criar um tipo de informação sensível personalizado**</span><span class="sxs-lookup"><span data-stu-id="18d36-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="18d36-112">Mas se precisar de identificar e proteger completamente um tipo diferente de informação sensível, pode criar um tipo de [informação sensível personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) na UI do Centro de Conformidade & Segurança.</span><span class="sxs-lookup"><span data-stu-id="18d36-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="18d36-113">**Criar um tipo de informação sensível personalizado em Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="18d36-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="18d36-114">Finalmente, se o UI não fornecer todas as opções de que necessita, pode criar um tipo de [informação sensível personalizado em Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="18d36-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="18d36-115">Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.</span><span class="sxs-lookup"><span data-stu-id="18d36-115">By starting with an XML file, you can use every option available.</span></span>
