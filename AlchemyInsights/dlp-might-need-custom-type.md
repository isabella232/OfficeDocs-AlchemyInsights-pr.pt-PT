---
title: DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712195"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="40f62-102">DLP pode precisar de um tipo personalizado</span><span class="sxs-lookup"><span data-stu-id="40f62-102">DLP might need a custom type</span></span>

<span data-ttu-id="40f62-103">**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).</span><span class="sxs-lookup"><span data-stu-id="40f62-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="40f62-104">**DLP pode exigir um tipo de informação personalizada**</span><span class="sxs-lookup"><span data-stu-id="40f62-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="40f62-105">Com uma política de prevenção de perda de dados (DLP), pode identificar e proteger dados sensíveis na sua organização.</span><span class="sxs-lookup"><span data-stu-id="40f62-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="40f62-106">Em alguns cenários, poderá ser necessário criar o seu próprio tipo **de** informação personalizada e sensível para proteger os dados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="40f62-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="40f62-107">Por exemplo, a sua organização poderá necessitar de identificar e proteger iDs de funcionários ou outros dados em algum formato específico do seu org. Em caso afirmativo, consulte os seguintes artigos para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="40f62-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="40f62-108">**Personalize um tipo de informação sensível incorporada**</span><span class="sxs-lookup"><span data-stu-id="40f62-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="40f62-109">Se um tipo de informação sensível incorporada satisfaça as suas necessidades com apenas alguns ajustes, pode [personalizar um tipo de informação sensível incorporada](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="40f62-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="40f62-110">Por exemplo, pode adicionar ou remover palavras-chave, ou adicionar ou remover provas de suporte, como uma data ou endereço.</span><span class="sxs-lookup"><span data-stu-id="40f62-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="40f62-111">**Criar um tipo de informação sensível personalizada**</span><span class="sxs-lookup"><span data-stu-id="40f62-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="40f62-112">Mas se precisar identificar e proteger um tipo diferente de informação sensível, pode [criar um tipo de informação sensível personalizada](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) na UI do Centro de Conformidade & de Segurança.</span><span class="sxs-lookup"><span data-stu-id="40f62-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="40f62-113">**Criar um tipo de informação sensível personalizada no Centro de Conformidade & Segurança PowerShell**</span><span class="sxs-lookup"><span data-stu-id="40f62-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="40f62-114">Finalmente, se a UI não fornecer todas as opções necessárias, pode [criar um tipo de informação sensível personalizada em Segurança & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="40f62-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="40f62-115">Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.</span><span class="sxs-lookup"><span data-stu-id="40f62-115">By starting with an XML file, you can use every option available.</span></span>
