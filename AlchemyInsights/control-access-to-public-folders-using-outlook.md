---
title: Controlar o acesso às pastas públicas através do Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816751"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="d4021-102">Controlar o acesso às pastas públicas através do Outlook</span><span class="sxs-lookup"><span data-stu-id="d4021-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="d4021-103">Para controlar os utilizadores que podem aceder às pastas públicas através do Outlook:</span><span class="sxs-lookup"><span data-stu-id="d4021-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="d4021-104">Utilizar o `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="d4021-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="d4021-105">$true: Permitir que os utilizadores acedam às pastas públicas no Outlook</span><span class="sxs-lookup"><span data-stu-id="d4021-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="d4021-106">$false: Impedir o acesso de utilizadores a pastas públicas no Outlook.</span><span class="sxs-lookup"><span data-stu-id="d4021-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="d4021-107">Este é o valor predefinido.</span><span class="sxs-lookup"><span data-stu-id="d4021-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="d4021-108">Nota: Este procedimento apenas pode controlar as ligações com o ambiente de trabalho do Outlook para clientes Windows.</span><span class="sxs-lookup"><span data-stu-id="d4021-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="d4021-109">Os utilizadores podem continuar a aceder a pastas públicas com o OWA ou o Outlook para Mac.</span><span class="sxs-lookup"><span data-stu-id="d4021-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="d4021-110">Para obter mais informações, consulte [Ligações Controladas a Pastas Públicas no Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="d4021-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
