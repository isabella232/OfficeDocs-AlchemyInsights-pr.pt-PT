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
# <a name="delete-orphaned-user-from-on-premises-server"></a>Eliminar utilizador órfão do servidor no local

Para remover um utilizador órfão, siga estes passos:

1. Sincronização do diretório de forças seguindo as instruções em Qual é a [identidade híbrida com o Azure Ative Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)

2. Para verificar a sincronização do diretório, veja [o que é a identidade híbrida com o Azure Ative Directory?](https://technet.microsoft.com/library/jj151797.aspx)

3. Se a sincronização funcionar corretamente, mas a eliminação do objeto ative directory não se propaga ao Azure AD, remova manualmente o objeto órfão utilizando um dos seguintes módulos de diretório ativo Azure para cmdlets Windows PowerShell:

    Remover-MsolContact  
    Remove-MsolGroup  
    Remover-MsolUser

    Por exemplo, para remover o ID do utilizador órfão john.smith@contoso.com, originalmente criados através da sincronização do diretório, executar o cmdlet:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com