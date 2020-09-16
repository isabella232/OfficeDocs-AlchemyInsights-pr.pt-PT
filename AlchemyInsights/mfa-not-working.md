---
title: Problemas com o MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755142"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="d3e30-102">Problemas com Azure MFA</span><span class="sxs-lookup"><span data-stu-id="d3e30-102">Issues with Azure MFA</span></span>
<span data-ttu-id="d3e30-103">Há algumas coisas para verificar se os utilizadores não podem iniciar sessão usando a autenticação de vários fatores (MFA)</span><span class="sxs-lookup"><span data-stu-id="d3e30-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="d3e30-104">O utilizador afetado pode estar bloqueado no Portal do Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="d3e30-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="d3e30-105">Se for esse o caso, as tentativas de autenticação para esse utilizador específico serão automaticamente negadas.</span><span class="sxs-lookup"><span data-stu-id="d3e30-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="d3e30-106">Por favor, siga os passos deste artigo para desbloqueá-los.</span><span class="sxs-lookup"><span data-stu-id="d3e30-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="d3e30-107">Se desbloquear o utilizador não ajudou ou o utilizador não está bloqueado, pode tentar reiniciar o MFA para o utilizador e passará novamente pelo processo de inscrição.</span><span class="sxs-lookup"><span data-stu-id="d3e30-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="d3e30-108">Por favor, siga os passos deste artigo.</span><span class="sxs-lookup"><span data-stu-id="d3e30-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="d3e30-109">Se esta for a primeira vez que ativou o MFA e os seus utilizadores não puderem iniciar sessão em clientes não-navegadores como o Outlook, Skype, etc, talvez a ADAL (Ative Directory Authentication Library) não esteja ativada na sua subscrição O365.</span><span class="sxs-lookup"><span data-stu-id="d3e30-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="d3e30-110">Neste caso, você precisará ligar-se ao Exchange Online Powershell e executar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="d3e30-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>