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
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393552"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="3fe80-102">Acesso condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="3fe80-102">Conditional Access with Intune</span></span>

<span data-ttu-id="3fe80-103">A utilização de **Acesso condicional** com Intune requer 3 passos:</span><span class="sxs-lookup"><span data-stu-id="3fe80-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="3fe80-104">Crie uma **Política de acesso condicional** que define quais os recursos que estão a ser protegidos e o que as condições que devem ser cumpridos para aceder aos recursos.</span><span class="sxs-lookup"><span data-stu-id="3fe80-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="3fe80-105">Por exemplo, um dispositivo tem de ser compatível com antes de aceder a correio electrónico da empresa.</span><span class="sxs-lookup"><span data-stu-id="3fe80-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="3fe80-106">Crie uma **Política de conformidade** para definir as definições que devem ser satisfeitas antes do dispositivo é considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="3fe80-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="3fe80-107">Por exemplo, um dispositivo tem de ter um pin de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="3fe80-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="3fe80-108">Assegurar a **Conformidade de políticas** e **Políticas de acesso condicional** são orientados para os grupos de utilizadores pretendidos.</span><span class="sxs-lookup"><span data-stu-id="3fe80-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="3fe80-109">Isto pode requerer a criação de grupos específicos de utilizadores do Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="3fe80-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="3fe80-110">Ler mais:</span><span class="sxs-lookup"><span data-stu-id="3fe80-110">Read more:</span></span>
  
- [<span data-ttu-id="3fe80-111">Condicionais procedimentos recomendados de acesso</span><span class="sxs-lookup"><span data-stu-id="3fe80-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="3fe80-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="3fe80-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

