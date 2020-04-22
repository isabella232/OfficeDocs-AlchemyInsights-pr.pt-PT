---
title: Acesso Condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706032"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="545eb-102">Acesso Condicional com Intune</span><span class="sxs-lookup"><span data-stu-id="545eb-102">Conditional Access with Intune</span></span>

<span data-ttu-id="545eb-103">Utilizar **o Acesso Condicional** com Intune requer 3 passos:</span><span class="sxs-lookup"><span data-stu-id="545eb-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="545eb-104">Criar uma Política de **Acesso Condicional** que defina quais os recursos que estão a ser protegidos e quais as condições a cumprir para aceder a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="545eb-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="545eb-105">Por exemplo, um dispositivo deve ser compatível antes de aceder a e-mails corporativos.</span><span class="sxs-lookup"><span data-stu-id="545eb-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="545eb-106">Crie uma Política de **Conformidade** para definir as definições que devem ser satisfeitas antes de o dispositivo ser considerado conforme.</span><span class="sxs-lookup"><span data-stu-id="545eb-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="545eb-107">Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="545eb-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="545eb-108">Garantir que tanto as Políticas de **Conformidade** como as Políticas de **Acesso Condicional** são direcionadas aos grupos de utilizadores pretendidos.</span><span class="sxs-lookup"><span data-stu-id="545eb-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="545eb-109">Isto pode exigir a criação de grupos específicos de utilizadores no Diretório Ativo Do Azure.</span><span class="sxs-lookup"><span data-stu-id="545eb-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="545eb-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="545eb-110">Read more:</span></span>
  
- [<span data-ttu-id="545eb-111">Acesso Condicional às melhores práticas</span><span class="sxs-lookup"><span data-stu-id="545eb-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="545eb-112">Começar com acesso condicional</span><span class="sxs-lookup"><span data-stu-id="545eb-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

