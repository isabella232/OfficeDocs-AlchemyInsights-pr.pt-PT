---
title: Problemas com base em problemas de assinatura sem emenda sem emenda (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714883"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="d1f27-102">Problemas com base em problemas de assinatura sem emenda sem emenda (SSO)</span><span class="sxs-lookup"><span data-stu-id="d1f27-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="d1f27-103">Para conhecer os fundamentos do SSO baseado em palavras-passe, consulte [a autenticação baseada em passwords com o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="d1f27-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="d1f27-104">**Configurar SSO baseado em palavras-passe**</span><span class="sxs-lookup"><span data-stu-id="d1f27-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="d1f27-105">[Configure o único sign-on baseado em palavra-passe](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Este artigo entra em mais detalhes sobre a opção SSO baseada em palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="d1f27-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="d1f27-106">Se a aplicação que está a adicionar necessitar de configuração personalizada e precisar de utilizar SSO baseado em palavra-passe, então este artigo é para si.</span><span class="sxs-lookup"><span data-stu-id="d1f27-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="d1f27-107">[Configure um único sinal baseado em palavra-passe para aplicações on-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - O Application Proxy suporta vários modos de entrada única.</span><span class="sxs-lookup"><span data-stu-id="d1f27-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="d1f27-108">O sign-on baseado em palavra-passe destina-se a aplicações que utilizem uma combinação de nome de utilizador/palavra-passe para autenticação.</span><span class="sxs-lookup"><span data-stu-id="d1f27-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="d1f27-109">Ao configurar o sign-on baseado em palavra-passe para a sua aplicação, os seus utilizadores têm de iniciar sação na aplicação no local uma vez.</span><span class="sxs-lookup"><span data-stu-id="d1f27-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="d1f27-110">Depois disso, o Azure Ative Directory armazena as informações de entrada e fornece-as automaticamente à aplicação quando os seus utilizadores acedem remotamente à sua aplicação.</span><span class="sxs-lookup"><span data-stu-id="d1f27-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="d1f27-111">Já devia ter publicado e testado a sua aplicação com o Application Proxy.</span><span class="sxs-lookup"><span data-stu-id="d1f27-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="d1f27-112">Caso contrário, siga os passos nas [aplicações de publicação utilizando o Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e, em seguida, continue a sua configuração de SSO baseado em palavra-passe para aplicações on-prem.</span><span class="sxs-lookup"><span data-stu-id="d1f27-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="d1f27-113">Para resolver problemas com sSO baseado em palavras-passe, consulte [o sign-on único baseado em resolução de palavras-passe em Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="d1f27-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
