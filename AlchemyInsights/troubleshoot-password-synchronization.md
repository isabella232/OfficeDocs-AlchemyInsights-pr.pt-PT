---
title: Sincronização de senha de resolução de problemas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732521"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f2915-102">Sincronização de senha de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="f2915-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f2915-103">Para resolver problemas em que nenhuma palavra-passe é sincronizada com a versão 1.1.614.0 do Azure AD Connect:</span><span class="sxs-lookup"><span data-stu-id="f2915-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="f2915-104">Abra uma nova sessão do Windows PowerShell no seu servidor Azure AD Connect com a opção **Executar como Administrador.**</span><span class="sxs-lookup"><span data-stu-id="f2915-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="f2915-105">Executar **Política de execução de séries Remotamente Assinada** ou Política de Execução de **Conjuntos sem restrições**.</span><span class="sxs-lookup"><span data-stu-id="f2915-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="f2915-106">Inicie o assistente Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f2915-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="f2915-107">Navegue na página **De Tarefas Adicionais,** selecione **Troubleshoot**, e clique **em Next**.</span><span class="sxs-lookup"><span data-stu-id="f2915-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="f2915-108">Na página Deresolução de Problemas, clique em Lançar para iniciar o menu de resolução de **problemas** no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f2915-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="f2915-109">No menu principal, selecione **Troubleshoot Password Synchronization**.</span><span class="sxs-lookup"><span data-stu-id="f2915-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="f2915-110">No menu sub, selecione **Password Synchronization não funciona**de todo .</span><span class="sxs-lookup"><span data-stu-id="f2915-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="f2915-111">**Compreenda os resultados da tarefa de resolução de problemas**</span><span class="sxs-lookup"><span data-stu-id="f2915-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="f2915-112">A tarefa de resolução de problemas realiza as seguintes verificações:</span><span class="sxs-lookup"><span data-stu-id="f2915-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="f2915-113">Valida que a funcionalidade de sincronização de palavras-passe está ativada para o seu inquilino Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f2915-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="f2915-114">Valida que o servidor Azure AD Connect não esteja em modo de encenação.</span><span class="sxs-lookup"><span data-stu-id="f2915-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="f2915-115">Para cada conector ativo de diretório existente no local (que corresponde a uma floresta de Diretório Ativo existente):</span><span class="sxs-lookup"><span data-stu-id="f2915-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="f2915-116">Valida que a função de sincronização da palavra-passe esteja ativada.</span><span class="sxs-lookup"><span data-stu-id="f2915-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="f2915-117">Pesquisas por eventos de batimentocardíaco de sincronização de palavras-passe nos registos do Windows Application Event.</span><span class="sxs-lookup"><span data-stu-id="f2915-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="f2915-118">Para cada domínio de Diretório Ativo sob o conector ative diretório no local:</span><span class="sxs-lookup"><span data-stu-id="f2915-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="f2915-119">Valida que o domínio é acessível a partir do servidor Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f2915-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="f2915-120">Valida que as contas de Serviços de Domínio de Diretório Ativo (AD DS) utilizadas pelo conector Ative Directory no local têm o nome de utilizador, palavra-passe e permissões corretas necessárias para a sincronização de palavras-passe.</span><span class="sxs-lookup"><span data-stu-id="f2915-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="f2915-121">Para obter mais ajuda na resolução de sincronização de palavras-passe, consulte a [sincronização da palavra-passe de Troubleshoot com a sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f2915-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  