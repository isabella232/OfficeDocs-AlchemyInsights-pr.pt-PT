---
title: Diretório ativo não sincronizando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265267"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="415ea-102">Diretório ativo não sincronizando</span><span class="sxs-lookup"><span data-stu-id="415ea-102">Active Directory not syncing</span></span>

<span data-ttu-id="415ea-103">Se estiver a receber erros de sincronização, tais como "nenhuma sincronização recente", ou notar o estado de sincronização do diretório no portal de administração do Office diz: "Última sincronizada há mais de 3 dias", pode ser que o AADConnect tenha configurações incorretas ou insuficientes permissões para realizar uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="415ea-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="415ea-104">Reinstalar o AADConnect utilizando definições expressas pode resolver o problema rapidamente:</span><span class="sxs-lookup"><span data-stu-id="415ea-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="415ea-105">[Descarregue a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="415ea-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="415ea-106">[Siga as instruções de instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="415ea-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="415ea-107">Para obter mais informações sobre as contas de serviço AADConnect, consulte [o Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="415ea-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
