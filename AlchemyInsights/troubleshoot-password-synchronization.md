---
title: Resolução de problemas de sincronização de palavra-passe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767187"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="79234-102">Resolução de problemas de sincronização de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="79234-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="79234-103">Para resolver problemas em que nenhuma palavra-passe é sincronizadas com Azure AD ligar versão 1.1.614.0 ou posterior:</span><span class="sxs-lookup"><span data-stu-id="79234-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="79234-104">Abra uma nova sessão do Windows PowerShell no servidor Azure AD ligar com a opção **Executar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="79234-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="79234-105">Executar **conjunto ExecutionPolicy RemoteSigned** ou **conjunto ExecutionPolicy ilimitado**.</span><span class="sxs-lookup"><span data-stu-id="79234-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="79234-106">Inicie o Assistente de ligação de AD Azure.</span><span class="sxs-lookup"><span data-stu-id="79234-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="79234-107">Navegue para o \* \* tarefas adicionais \* \* página, seleccione \* \* resolução de problemas \* \* e clique em **seguinte**.</span><span class="sxs-lookup"><span data-stu-id="79234-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="79234-108">Na página de resolução de problemas, clique em menu **Iniciar para iniciar a resolução de problemas** no PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79234-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="79234-109">No menu principal, seleccione a **Resolução de problemas de sincronização de palavra-passe**.</span><span class="sxs-lookup"><span data-stu-id="79234-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="79234-110">No menu ' sub ', seleccione a **sincronização de palavra-passe não funciona em todos os**.</span><span class="sxs-lookup"><span data-stu-id="79234-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="79234-111">**Compreender os resultados da tarefa de resolução de problemas**</span><span class="sxs-lookup"><span data-stu-id="79234-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="79234-112">A tarefa de resolução de problemas efectua as seguintes verificações:</span><span class="sxs-lookup"><span data-stu-id="79234-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="79234-113">Confirma que a funcionalidade de sincronização de palavra-passe está activada para o locatário Azure AD.</span><span class="sxs-lookup"><span data-stu-id="79234-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="79234-114">Confirma que o servidor de Azure AD ligar não está no modo de teste.</span><span class="sxs-lookup"><span data-stu-id="79234-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="79234-115">Para cada existentes no local conector do Active Directory (que corresponde a uma floresta existente do Active Directory):</span><span class="sxs-lookup"><span data-stu-id="79234-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="79234-116">Confirma que a funcionalidade de sincronização de palavra-passe está activada.</span><span class="sxs-lookup"><span data-stu-id="79234-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="79234-117">Procura de eventos de heartbeat de sincronização de palavra-passe nos registos de eventos de aplicações do Windows.</span><span class="sxs-lookup"><span data-stu-id="79234-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="79234-118">Para cada domínio do Active Directory com o Active Directory connector no local:</span><span class="sxs-lookup"><span data-stu-id="79234-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="79234-119">Confirma que o domínio é acessível a partir do servidor Azure AD ligar.</span><span class="sxs-lookup"><span data-stu-id="79234-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="79234-120">Confirma-se de que as contas de serviços de domínio do Active Directory (AD DS) utilizadas pelo conector Active Directory no local tem o nome de utilizador correcto, palavra-passe e permissões necessárias para a sincronização de palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="79234-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="79234-121">Para obter mais ajuda, resolução de problemas de sincronização de palavra-passe, consulte [sincronização de palavra-passe de resolução de problemas com sincronização Azure AD ligar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="79234-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

