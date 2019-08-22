---
title: Problemas relacionados com AMF
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545187"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="01f1d-102">Problemas relacionados com AMF</span><span class="sxs-lookup"><span data-stu-id="01f1d-102">Issues with MFA</span></span>
<span data-ttu-id="01f1d-103">Existem algumas coisas para verificar se os utilizadores não podem iniciar sessão utilizando autenticação multi-factores (AMF)</span><span class="sxs-lookup"><span data-stu-id="01f1d-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="01f1d-104">O utilizador afectado poderão ser bloqueado no Portal de directório Active Azure.</span><span class="sxs-lookup"><span data-stu-id="01f1d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="01f1d-105">Se for esse o caso, tentativas de autenticação para esse utilizador específico será automaticamente recusado.</span><span class="sxs-lookup"><span data-stu-id="01f1d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="01f1d-106">Siga os passos neste artigo para desbloqueá-los.</span><span class="sxs-lookup"><span data-stu-id="01f1d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="01f1d-107">Se desbloquear o utilizador ajudou ou o utilizador não está bloqueado pode tentar repor AMF para o utilizador e que aceitem através do processo de inscrição novamente.</span><span class="sxs-lookup"><span data-stu-id="01f1d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="01f1d-108">Siga os passos descritos neste artigo.</span><span class="sxs-lookup"><span data-stu-id="01f1d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="01f1d-109">Se esta for a primeira vez AMF activado e os utilizadores não conseguem iniciar sessão para clientes não browsers, tais como o Outlook, Skype, etc, talvez ADAL (Active Directory autenticação biblioteca) não está activada na sua subscrição de O365.</span><span class="sxs-lookup"><span data-stu-id="01f1d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="01f1d-110">Neste caso terá de ligar ao Exchange Online Powershell e executar este cmdlet:  *conjunto-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="01f1d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>