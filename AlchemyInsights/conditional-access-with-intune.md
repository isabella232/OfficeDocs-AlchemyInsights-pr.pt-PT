---
title: Acesso condicional com intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505005"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="55cf1-102">Acesso condicional com intune</span><span class="sxs-lookup"><span data-stu-id="55cf1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="55cf1-103">O **uso do Acesso Condicional** com o Intune requer 3 etapas:</span><span class="sxs-lookup"><span data-stu-id="55cf1-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="55cf1-104">Crie uma Política de **Acesso Condicional** que defina quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.</span><span class="sxs-lookup"><span data-stu-id="55cf1-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="55cf1-105">Por exemplo, um dispositivo deve estar em conformidade antes de acessar o e-mail corporativo.</span><span class="sxs-lookup"><span data-stu-id="55cf1-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="55cf1-106">Crie uma política de **conformidade** para definir configurações que devem ser atendidas antes que o dispositivo seja considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="55cf1-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="55cf1-107">Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível.</span><span class="sxs-lookup"><span data-stu-id="55cf1-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="55cf1-108">Garantir que as **Políticas** de Conformidade e as **Políticas** de Acesso Condicional sejam direcionadas aos grupos de usuários desejados.</span><span class="sxs-lookup"><span data-stu-id="55cf1-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="55cf1-109">Isso pode exigir a criação de grupos específicos de usuários no Diretório Ativo Do Azure.</span><span class="sxs-lookup"><span data-stu-id="55cf1-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="55cf1-110">Leia mais:</span><span class="sxs-lookup"><span data-stu-id="55cf1-110">Read more:</span></span>
  
- [<span data-ttu-id="55cf1-111">Melhores práticas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="55cf1-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="55cf1-112">Começar com acesso condicional</span><span class="sxs-lookup"><span data-stu-id="55cf1-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

