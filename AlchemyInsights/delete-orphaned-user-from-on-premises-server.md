---
title: Eliminar utilizador órfão do servidor no local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198591"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="2ef97-102">Eliminar utilizador órfão do servidor no local</span><span class="sxs-lookup"><span data-stu-id="2ef97-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="2ef97-103">Para remover um utilizador órfão, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="2ef97-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="2ef97-104">Sincronização do diretório de forças seguindo as instruções em Qual é a [identidade híbrida com o Azure Ative Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)</span><span class="sxs-lookup"><span data-stu-id="2ef97-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="2ef97-105">Para verificar a sincronização do diretório, veja [o que é a identidade híbrida com o Azure Ative Directory?](https://technet.microsoft.com/library/jj151797.aspx)</span><span class="sxs-lookup"><span data-stu-id="2ef97-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="2ef97-106">Se a sincronização funcionar corretamente, mas a eliminação do objeto ative directory não se propaga ao Azure AD, remova manualmente o objeto órfão utilizando um dos seguintes módulos de diretório ativo Azure para cmdlets Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2ef97-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="2ef97-107">Remover-MsolContact</span><span class="sxs-lookup"><span data-stu-id="2ef97-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="2ef97-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="2ef97-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="2ef97-109">Remover-MsolUser</span><span class="sxs-lookup"><span data-stu-id="2ef97-109">Remove-MsolUser</span></span>

    <span data-ttu-id="2ef97-110">Por exemplo, para remover o ID do utilizador órfão john.smith@contoso.com, originalmente criados através da sincronização do diretório, executar o cmdlet:</span><span class="sxs-lookup"><span data-stu-id="2ef97-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="2ef97-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="2ef97-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>