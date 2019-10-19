---
title: Acesso condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36505005"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b35c7-102">Acesso condicional com o Intune</span><span class="sxs-lookup"><span data-stu-id="b35c7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b35c7-103">Usar o **acesso condicional** com o Intune requer 3 etapas:</span><span class="sxs-lookup"><span data-stu-id="b35c7-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="b35c7-104">Crie uma **política de acesso condicional** que defina quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.</span><span class="sxs-lookup"><span data-stu-id="b35c7-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="b35c7-105">Por exemplo, um dispositivo deve ser compatível antes de acessar o email corporativo.</span><span class="sxs-lookup"><span data-stu-id="b35c7-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="b35c7-106">Crie uma **política de conformidade** para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="b35c7-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b35c7-107">Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="b35c7-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="b35c7-108">Garantir que as **diretivas de conformidade** e as diretivas de **acesso condicional** sejam direcionadas para os grupos de usuários desejados.</span><span class="sxs-lookup"><span data-stu-id="b35c7-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="b35c7-109">Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b35c7-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="b35c7-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="b35c7-110">Read more:</span></span>
  
- [<span data-ttu-id="b35c7-111">Práticas recomendadas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="b35c7-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="b35c7-112">Introdução ao acesso condicional</span><span class="sxs-lookup"><span data-stu-id="b35c7-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

