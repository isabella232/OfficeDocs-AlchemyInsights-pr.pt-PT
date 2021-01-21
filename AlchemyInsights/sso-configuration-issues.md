---
title: Problemas de configuração SSO
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: 5ab56ec1eda10ea059e600e8933ce85bb143b76e
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901353"
---
# <a name="sso-configuration-issues"></a><span data-ttu-id="b0e6f-102">Problemas de configuração SSO</span><span class="sxs-lookup"><span data-stu-id="b0e6f-102">SSO configuration issues</span></span>

1. <span data-ttu-id="b0e6f-103">Siga o [Quickstart: Configure propriedades para um](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guia de aplicações para configurar a sua aplicação.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-103">Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.</span></span>
2. <span data-ttu-id="b0e6f-104">Dependendo da aplicação e [da opção de inscrição única](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que escolheu, siga as orientações apropriadas abaixo: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-104">Depending on the application and [Single sign-on option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) that you chose, follow the appropriate guidance below: a.</span></span> <span data-ttu-id="b0e6f-105">Para configurar um **pedido no local** para um único **sign-on (SSO) baseado em SAML,** consulte [o auto-sign-on da SAML para aplicações no local com proxy de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span><span class="sxs-lookup"><span data-stu-id="b0e6f-105">To configure an **on-premises application** for **SAML-based single sign-on (SSO)**, see [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span></span>
    <span data-ttu-id="b0e6f-106">b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-106">b.</span></span> <span data-ttu-id="b0e6f-107">Para configurar uma **aplicação** em nuvem para **SSO baseado em palavras-passe,** consulte [configurar a palavra-passe de um único sinal](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="b0e6f-107">To configure a **cloud application** for **password-based SSO**, see [Configure password single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span></span>
    <span data-ttu-id="b0e6f-108">c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-108">c.</span></span> <span data-ttu-id="b0e6f-109">Para configurar um **pedido no local** para **SSO através de Application Proxy**, consulte [abotoação de palavra-passe para um único sinal de acesso com Proxy de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="b0e6f-109">To configure an **on-premises application** for **SSO through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
3. <span data-ttu-id="b0e6f-110">**Problemas de resolução de problemas Problemas Aplicação Problemas de procuração**: Recomendamos que comece a rever o fluxo de resolução de problemas - [problemas de conector de procuração de aplicação de depuração](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) - para determinar se os conectores de procuração de aplicação estão configurados corretamente.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-110">**Troubleshooting Application Proxy issues**: We recommend that you start with reviewing the troubleshooting flow - [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) - to determine if application proxy connectors are configured correctly.</span></span> <span data-ttu-id="b0e6f-111">Se ainda tiver problemas em ligar-se à aplicação, siga os passos de resolução de problemas em problemas de [aplicação de depuração](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="b0e6f-111">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="b0e6f-112">Pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) realizando os seguintes passos de depurar o navegador: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-112">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by performing the following browser debug steps: a.</span></span> <span data-ttu-id="b0e6f-113">Lance o navegador e navegue para a aplicação web.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-113">Launch the browser and browse to the web app.</span></span>
    <span data-ttu-id="b0e6f-114">b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-114">b.</span></span> <span data-ttu-id="b0e6f-115">Pressione **f12** para trazer a consola de depurg.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-115">Press **F12** to bring up the debug console.</span></span>
    <span data-ttu-id="b0e6f-116">c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-116">c.</span></span> <span data-ttu-id="b0e6f-117">Tente reproduzir a transação e reveja a mensagem da consola.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-117">Try to reproduce the transaction and review the console message.</span></span> <span data-ttu-id="b0e6f-118">Uma violação do CORS produz um erro de consola sobre a origem.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-118">A CORS violation produces a console error about origin.</span></span>
    <span data-ttu-id="b0e6f-119">d.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-119">d.</span></span> <span data-ttu-id="b0e6f-120">Alguns problemas do CORS não podem ser resolvidos, como a expiração do token de acesso quando a sua aplicação redireciona para login.microsoftonline.com para autenticação.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-120">Some CORS issues can't be resolved, such as expiration of the access token when your app redirects to login.microsoftonline.com for authentication.</span></span> <span data-ttu-id="b0e6f-121">Como resultado da expiração do token de acesso, a chamada CORS falha.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-121">As a result of the access token expiration, the CORS call then fails.</span></span> <span data-ttu-id="b0e6f-122">Uma solução alternativa para este cenário é prolongar a vida útil do token de acesso, para evitar que expire durante a sessão do utilizador.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-122">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="b0e6f-123">Para obter mais informações sobre como fazê-lo, consulte [as vidas de token configurantes na plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="b0e6f-123">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
4. <span data-ttu-id="b0e6f-124">**SSO baseado em problemas baseado em SAML**: Recomendamos que se inscreva [problemas de sessão em aplicações configuradas com base em SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para encontrar as soluções para os problemas que você é mais provável encontrar.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-124">**Troubleshooting SAML-based SSO**: We recommend checking [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to find the solutions to the issues you are most likely to encounter.</span></span>
5. <span data-ttu-id="b0e6f-125">**SSO baseado em resolução de problemas baseado em palavras-passe**: Recomendamos que verifique o [único sinal baseado em Ad baseado em resolução de palavras-passe para](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) encontrar as soluções para os problemas que você é mais provável encontrar.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-125">**Troubleshooting password-based SSO**: We recommend checking [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to find the solutions to the issues you are most likely to encounter.</span></span>
6. <span data-ttu-id="b0e6f-126">**Recebi um erro de configuração**: Para resolver erros de configuração de resolução de problemas, recomendamos verificar os seguintes artigos: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-126">**I received a configuration error**: To troubleshoot configuration errors, we recommend checking the following articles: a.</span></span> <span data-ttu-id="b0e6f-127">[Problemas de inscrição em aplicações configuradas com base em SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-127">[Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b.</span></span> <span data-ttu-id="b0e6f-128">[As credenciais são preenchidas, mas a extensão não as submete](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-128">[Credentials are filled in, but the extension does not submit them](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c.</span></span> <span data-ttu-id="b0e6f-129">[As credenciais são preenchidas e submetidas, mas a página indica que as credenciais estão incorretas.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="b0e6f-129">[Credentials are filled in and submitted, but the page indicates the credentials are incorrect](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d.</span></span> [<span data-ttu-id="b0e6f-130">Uma página de aplicação mostra uma mensagem de erro após o utilizador assinar em</span><span class="sxs-lookup"><span data-stu-id="b0e6f-130">An app page shows an error message after the user signs in</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. <span data-ttu-id="b0e6f-131">**Estou a ter problemas em integrar o Seamless SSO com as minhas aplicações no local**: Para resolver problemas relacionados com a integração do SSO sem emenda com aplicações no local, recomendamos verificar os seguintes artigos: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-131">**I am having issues integrating Seamless SSO with my on-premises apps**: To troubleshoot issues regarding integration of Seamless SSO with on-premises apps, we recommend checking the following articles: a.</span></span> <span data-ttu-id="b0e6f-132">[Como configurar um único sinal de inscrição para uma aplicação de procuração de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-132">[How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b.</span></span> <span data-ttu-id="b0e6f-133">[SAML único sinal de inscrição para aplicações no local com Aplicação Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-133">[SAML single sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c.</span></span> <span data-ttu-id="b0e6f-134">[Compreender e resolver as questões de Proxy CORS da Aplicação Ative Azure.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)</span><span class="sxs-lookup"><span data-stu-id="b0e6f-134">[Understand and solve Azure Active Directory Application Proxy CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d.</span></span> [<span data-ttu-id="b0e6f-135">Resolução de problemas Kerberos limitou configurações da delegação para aplicação proxy</span><span class="sxs-lookup"><span data-stu-id="b0e6f-135">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. <span data-ttu-id="b0e6f-136">**Preciso corrigir as reclamações ou prolongar a vida de um símbolo. Preciso de alterar a duração de uma sessão:** Para o fazer, recomendamos verificar os seguintes artigos: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-136">**I need to fix the claims or extend the lifetime of a token. I need to change the length of a session**: To do this, we recommend checking the following articles: a.</span></span> <span data-ttu-id="b0e6f-137">[Personalize as reclamações da SAML enviadas para uma aplicação](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-137">[Customize SAML claims sent to an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b.</span></span> <span data-ttu-id="b0e6f-138">[Trabalhar com aplicações conscientes de reclamações](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-138">[Working with claims-aware apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c.</span></span> <span data-ttu-id="b0e6f-139">[Vidas de token configuradas na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-139">[Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d.</span></span> <span data-ttu-id="b0e6f-140">[Configurar gestão da sessão de autenticação com Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-140">[Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e.</span></span> [<span data-ttu-id="b0e6f-141">Definições de cookies para aceder a aplicações no local</span><span class="sxs-lookup"><span data-stu-id="b0e6f-141">Cookie settings for accessing on-premises applications</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. <span data-ttu-id="b0e6f-142">**Preciso de ajuda para gerir o acesso dos meus utilizadores e utilizadores convidados (B2B):** Para informações detalhadas sobre a gestão do acesso dos utilizadores e dos utilizadores dos hóspedes, recomendamos verificar os seguintes artigos: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-142">**I need help managing my user's and guest users' (B2B) access**: For detailed information on managing user's and guest user's access, we recommend checking the following articles: a.</span></span> <span data-ttu-id="b0e6f-143">[Gerir o acesso às apps](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-143">[Managing access to apps](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b.</span></span> <span data-ttu-id="b0e6f-144">[Gerir a atribuição do utilizador para uma aplicação no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-144">[Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c.</span></span> <span data-ttu-id="b0e6f-145">[Configure aplicativos SaaS para colaboração B2B](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-145">[Configure SaaS apps for B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d.</span></span> <span data-ttu-id="b0e6f-146">[Grant B2B utilizadores em Azure AD acesso às suas aplicações no local](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-146">[Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e.</span></span> [<span data-ttu-id="b0e6f-147">Conceder contas de parceiros geridos localmente acesso a recursos em nuvem usando a colaboração Azure AD B2B</span><span class="sxs-lookup"><span data-stu-id="b0e6f-147">Grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration</span></span>](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. <span data-ttu-id="b0e6f-148">**Quero personalizar as minhas aplicações**: Para informações detalhadas sobre a personalização de apps, recomendamos verificar os seguintes artigos: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-148">**I want to customize my apps**: For detailed information on customizing apps, we recommend checking the following articles: a.</span></span> <span data-ttu-id="b0e6f-149">[Configure domínios personalizados com Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-149">[Configure custom domains with Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b.</span></span> <span data-ttu-id="b0e6f-150">[Desaça uma página inicial personalizada para aplicações publicadas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-150">[Set a custom home page for published apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c.</span></span> [<span data-ttu-id="b0e6f-151">Aplicações wildcard</span><span class="sxs-lookup"><span data-stu-id="b0e6f-151">Wildcard applications</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. <span data-ttu-id="b0e6f-152">**Estou a ter problemas em migrar a minha app de AD FS para Azure**: Para resolver problemas encontrados durante a migração da sua app de AD FS para Azure, recomendamos verificar os seguintes artigos: a.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-152">**I'm having issues migrating my app from AD FS to Azure**: To troubleshoot issues encountered during migration of your app from AD FS to Azure, we recommend checking the following articles: a.</span></span> <span data-ttu-id="b0e6f-153">[Autenticação de aplicações móveis dos Serviços da Federação de Diretórios Ativos para o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b.</span><span class="sxs-lookup"><span data-stu-id="b0e6f-153">[Moving application authentication from Active Directory Federation Services to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b.</span></span> [<span data-ttu-id="b0e6f-154">Recursos para aplicações migratórias para o Azure Ative Directory</span><span class="sxs-lookup"><span data-stu-id="b0e6f-154">Resources for migrating applications to Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)
