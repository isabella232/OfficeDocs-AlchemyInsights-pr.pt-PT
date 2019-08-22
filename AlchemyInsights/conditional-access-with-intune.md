---
title: Acesso condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505005"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="83b98-102">Acesso condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="83b98-102">Conditional Access with Intune</span></span>

<span data-ttu-id="83b98-103">A utilização de **Acesso condicional** com Intune requer 3 passos:</span><span class="sxs-lookup"><span data-stu-id="83b98-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="83b98-104">Crie uma **Política de acesso condicional** que define quais os recursos que estão a ser protegidos e o que as condições que devem ser cumpridos para aceder aos recursos.</span><span class="sxs-lookup"><span data-stu-id="83b98-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="83b98-105">Por exemplo, um dispositivo tem de ser compatível com antes de aceder a correio electrónico da empresa.</span><span class="sxs-lookup"><span data-stu-id="83b98-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="83b98-106">Crie uma **Política de conformidade** para definir as definições que devem ser satisfeitas antes do dispositivo é considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="83b98-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="83b98-107">Por exemplo, um dispositivo tem de ter um pin de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="83b98-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="83b98-108">Assegurar a **Conformidade de políticas** e **Políticas de acesso condicional** são orientados para os grupos de utilizadores pretendidos.</span><span class="sxs-lookup"><span data-stu-id="83b98-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="83b98-109">Isto pode requerer a criação de grupos específicos de utilizadores do Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="83b98-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="83b98-110">Ler mais:</span><span class="sxs-lookup"><span data-stu-id="83b98-110">Read more:</span></span>
  
- [<span data-ttu-id="83b98-111">Condicionais procedimentos recomendados de acesso</span><span class="sxs-lookup"><span data-stu-id="83b98-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="83b98-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="83b98-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

