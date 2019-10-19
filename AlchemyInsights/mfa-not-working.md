---
title: Problemas com MFA
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545187"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="dcd95-102">Problemas com MFA</span><span class="sxs-lookup"><span data-stu-id="dcd95-102">Issues with MFA</span></span>
<span data-ttu-id="dcd95-103">Há algumas coisas para verificar se os usuários não podem fazer login usando a autenticação multifator (MFA)</span><span class="sxs-lookup"><span data-stu-id="dcd95-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="dcd95-104">O usuário afetado pode ser bloqueado no portal do Active Directory do Azure.</span><span class="sxs-lookup"><span data-stu-id="dcd95-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="dcd95-105">Se for esse o caso, as tentativas de autenticação para esse usuário específico serão negadas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="dcd95-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="dcd95-106">Por favor, siga os passos neste artigo para desbloqueá-los.</span><span class="sxs-lookup"><span data-stu-id="dcd95-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="dcd95-107">Se o desbloqueio do usuário não ajudar ou o usuário não estiver bloqueado, você poderá tentar redefinir a MFA para o usuário e eles irão passar pelo processo de registro novamente.</span><span class="sxs-lookup"><span data-stu-id="dcd95-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="dcd95-108">Por favor, siga os passos neste artigo.</span><span class="sxs-lookup"><span data-stu-id="dcd95-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="dcd95-109">Se esta for a primeira vez que você habilitou o MFA e seus usuários não conseguem fazer logon em clientes que não sejam navegadores, como Outlook, Skype, etc, talvez a ADAL (biblioteca de autenticação do Active Directory) não esteja habilitada na sua assinatura do O365.</span><span class="sxs-lookup"><span data-stu-id="dcd95-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="dcd95-110">Nesse caso, será necessário conectar-se ao PowerShell do Exchange Online e executar este cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="dcd95-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>