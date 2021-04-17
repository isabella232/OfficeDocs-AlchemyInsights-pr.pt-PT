---
title: Diretório Ativo não sincronização
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822862"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="72edb-102">Diretório Ativo não sincronização</span><span class="sxs-lookup"><span data-stu-id="72edb-102">Active Directory not syncing</span></span>

<span data-ttu-id="72edb-103">Se estiver a receber erros de sincronização, como "nenhuma sincronização recente", ou notar o estado de sincronização do diretório no portal de administração do Office diz: "A última sincronização foi há mais de 3 dias", pode ser que a AADConnect tenha configurações incorretas ou permissões insuficientes para realizar uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="72edb-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="72edb-104">Reinstalar o AADConnect utilizando definições expressas pode resolver o problema rapidamente:</span><span class="sxs-lookup"><span data-stu-id="72edb-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="72edb-105">[Descarregue a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="72edb-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="72edb-106">[Siga as instruções de instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="72edb-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="72edb-107">Para obter mais informações sobre as contas do serviço AADConnect, consulte [Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="72edb-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
