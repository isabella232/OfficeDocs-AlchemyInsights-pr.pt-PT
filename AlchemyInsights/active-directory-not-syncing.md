---
title: O Active Directory não está a ser syncing
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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930986"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="83963-102">O Active Directory não está a ser syncing</span><span class="sxs-lookup"><span data-stu-id="83963-102">Active Directory not syncing</span></span>

<span data-ttu-id="83963-103">Se estiver a receber erros de sincronização, como "sem sincronização recente", ou repare que o estado de sincronização de diretórios no portal de administração do Office indica "Última sincronização há mais de 3 dias", pode ser que o AADConnect tem definições incorretas ou permissões insuficientes para efetuar uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="83963-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="83963-104">Reinstalar o AADConnect através de definições rápidas pode resolver o problema rapidamente:</span><span class="sxs-lookup"><span data-stu-id="83963-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="83963-105">[Transfira a versão mais recente do AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="83963-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="83963-106">[Siga as instruções de instalação rápida.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="83963-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="83963-107">O Azure AD Connect tem de ser instalado no Windows Server 2012 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="83963-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="83963-108">Este servidor deve ser unido ao domínio e pode ser um controlador de domínio ou um servidor membro.</span><span class="sxs-lookup"><span data-stu-id="83963-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="83963-109">Para ver uma lista completa do Azure AD Ligação requisitos e pré-requisitos, reveja os Pré-requisitos do [Azure AD Ligação.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="83963-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="83963-110">Para obter mais informações sobre contas de serviço do AADConnect, consulte [O Azure AD Ligação: Contas e permissões.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="83963-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
