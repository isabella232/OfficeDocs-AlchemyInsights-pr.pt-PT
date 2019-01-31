---
title: Acesso condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662338"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f62cb-102">Acesso condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="f62cb-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f62cb-103">A utilização de **Acesso condicional** com Intune requer 3 passos:</span><span class="sxs-lookup"><span data-stu-id="f62cb-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="f62cb-p101">Crie uma **Política de acesso condicional** que define quais os recursos que estão a ser protegidos e o que as condições que devem ser cumpridos para aceder aos recursos. Por exemplo, um dispositivo tem de ser compatível com antes de aceder a correio electrónico da empresa.</span><span class="sxs-lookup"><span data-stu-id="f62cb-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="f62cb-p102">Crie uma **Política de conformidade** para definir as definições que devem ser satisfeitas antes do dispositivo é considerado compatível. Por exemplo, um dispositivo tem de ter um pin de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="f62cb-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="f62cb-p103">Assegurar a **Conformidade de políticas** e **Políticas de acesso condicional** são orientados para os grupos de utilizadores pretendidos. Isto pode requerer a criação de grupos específicos de utilizadores do Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="f62cb-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="f62cb-110">Ler mais:</span><span class="sxs-lookup"><span data-stu-id="f62cb-110">Read more:</span></span>
  
- [<span data-ttu-id="f62cb-111">Condicionais procedimentos recomendados de acesso</span><span class="sxs-lookup"><span data-stu-id="f62cb-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="f62cb-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="f62cb-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

