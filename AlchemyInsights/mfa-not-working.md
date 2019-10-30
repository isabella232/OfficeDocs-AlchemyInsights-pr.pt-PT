---
title: Problemas com mfa
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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768848"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="cd25a-102">Problemas com o Azure MFA</span><span class="sxs-lookup"><span data-stu-id="cd25a-102">Issues with Azure MFA</span></span>
<span data-ttu-id="cd25a-103">Há algumas coisas para verificar se os usuários não podem fazer login usando autenticação multifator (MFA)</span><span class="sxs-lookup"><span data-stu-id="cd25a-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cd25a-104">O usuário afetado pode ser bloqueado no Portal de Diretório Ativo do Azure.</span><span class="sxs-lookup"><span data-stu-id="cd25a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cd25a-105">Se for esse o caso, as tentativas de autenticação para esse usuário específico serão automaticamente negadas.</span><span class="sxs-lookup"><span data-stu-id="cd25a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cd25a-106">Por favor, siga os passos deste artigo para desbloqueá-los.</span><span class="sxs-lookup"><span data-stu-id="cd25a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cd25a-107">Se desbloquear o usuário não ajudou ou o usuário não estiver bloqueado, você pode tentar redefinir o MFA para o usuário e eles passarão pelo processo de inscrição novamente.</span><span class="sxs-lookup"><span data-stu-id="cd25a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cd25a-108">Por favor, siga os passos deste artigo.</span><span class="sxs-lookup"><span data-stu-id="cd25a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cd25a-109">Se esta for a primeira vez que você habilitado MFA e seus usuários são incapazes de fazer login em clientes não-navegadores, como Outlook, Skype, etc, talvez ADAL (Active Directory Authentication Library) não está habilitado em sua assinatura O365.</span><span class="sxs-lookup"><span data-stu-id="cd25a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cd25a-110">Neste caso, você precisará se conectar à Troca online powershell e executar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="cd25a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>