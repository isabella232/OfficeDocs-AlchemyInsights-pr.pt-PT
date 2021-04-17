---
title: Não é possível aceder a pastas públicas
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819523"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="4d907-102">Outlook não pode ligar-se a pastas públicas</span><span class="sxs-lookup"><span data-stu-id="4d907-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="4d907-103">Se o acesso a pastas públicas não estiver a funcionar para alguns utilizadores, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4d907-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="4d907-104">Ligue-se ao EXO PowerShell e configuure o parâmetro DefaultPublicFolderMailbox na conta de utilizador do problema para corresponder ao parâmetro numa conta de utilizador de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4d907-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="4d907-105">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="4d907-105">Example:</span></span>

<span data-ttu-id="4d907-106">| de Get-Mailbox WorkingUser ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="4d907-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="4d907-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="4d907-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="4d907-108">Espere pelo menos uma hora para a mudança fazer efeito.</span><span class="sxs-lookup"><span data-stu-id="4d907-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="4d907-109">Se o problema se mantiver, por favor siga [este procedimento](https://aka.ms/pfcte) para resolver problemas de acesso a pastas públicas usando o Outlook.</span><span class="sxs-lookup"><span data-stu-id="4d907-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="4d907-110">**Para controlar quais os utilizadores que podem aceder a pastas públicas utilizando o Outlook:**</span><span class="sxs-lookup"><span data-stu-id="4d907-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="4d907-111">Utilize Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ou $false</span><span class="sxs-lookup"><span data-stu-id="4d907-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="4d907-112">$true: Permitir aos utilizadores aceder a pastas públicas no Outlook</span><span class="sxs-lookup"><span data-stu-id="4d907-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="4d907-113">$false: Impedir o acesso do utilizador a pastas públicas no Outlook.</span><span class="sxs-lookup"><span data-stu-id="4d907-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="4d907-114">This is the default value.</span><span class="sxs-lookup"><span data-stu-id="4d907-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="4d907-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="4d907-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="4d907-116">**Nota** Este procedimento só pode controlar as ligações com o desktop do Outlook para os clientes Windows.</span><span class="sxs-lookup"><span data-stu-id="4d907-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="4d907-117">Um utilizador pode continuar a aceder a pastas públicas utilizando OWA ou Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="4d907-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="4d907-118">Para obter mais informações, consulte [o Anúncio de Suporte para Ligações Controladas a Pastas Públicas no Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="4d907-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>