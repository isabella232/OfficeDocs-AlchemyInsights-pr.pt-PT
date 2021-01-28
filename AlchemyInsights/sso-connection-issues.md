---
title: Problemas de conexão SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935156"
---
# <a name="sso-connection-issues"></a><span data-ttu-id="76244-102">Problemas de conexão SSO</span><span class="sxs-lookup"><span data-stu-id="76244-102">SSO Connection Issues</span></span>

1. <span data-ttu-id="76244-103">Siga o [Quickstart: Configure propriedades para um](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guia de aplicações para configurar a sua aplicação.</span><span class="sxs-lookup"><span data-stu-id="76244-103">Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.</span></span>
2. <span data-ttu-id="76244-104">Dependendo da aplicação e da [opção de inscrição única](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que escolheu, siga as orientações apropriadas abaixo:</span><span class="sxs-lookup"><span data-stu-id="76244-104">Depending on the application and [Single sign-on option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) you chose, follow the appropriate guidance below:</span></span>
    - <span data-ttu-id="76244-105">Para configurar um pedido no local para um único **sign-on** **baseado em SAML,** consulte [a SAML single-sign-on para aplicações no local com Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span><span class="sxs-lookup"><span data-stu-id="76244-105">To configure an **on-premises application** for **SAML-based single sign-on**, see [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span></span>
    - <span data-ttu-id="76244-106">Para configurar uma **aplicação** em nuvem para **um único sinal de assinatura baseado em palavra-passe,** consulte  [configurar a palavra-passe de um único sinal](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="76244-106">To configure a **cloud application** for **password-based single sign-on**, see  [Configure password single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span></span>
    - <span data-ttu-id="76244-107">Para configurar um **pedido no local** para um único sinal de acesso através de **Aplicação Proxy**, consulte [abotoação de palavra-passe para um único sinal de acesso com procuração de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="76244-107">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
3. <span data-ttu-id="76244-108">**Problemas de resolução de problemas Problemas Aplicação Problemas de procuração**: recomendamos que comece a rever o fluxo de resolução [de problemas, problemas de Conector de Procuração de Aplicações de Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), para determinar se os conectores de procuração de aplicação estão configurados corretamente.</span><span class="sxs-lookup"><span data-stu-id="76244-108">**Troubleshooting Application Proxy issues**: we recommend you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="76244-109">Se ainda tiver problemas em ligar-se à aplicação, siga o fluxo de resolução de problemas em problemas de [aplicação de depuração](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="76244-109">If you are still having trouble connecting to the application, follow the troubleshooting flow in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="76244-110">Pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizando ferramentas de depuragem de navegador:</span><span class="sxs-lookup"><span data-stu-id="76244-110">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using browser debug tools:</span></span>
    - <span data-ttu-id="76244-111">Lance o navegador e navegue para a aplicação web.</span><span class="sxs-lookup"><span data-stu-id="76244-111">Launch the browser and browse to the web app.</span></span>
    - <span data-ttu-id="76244-112">Pressione **f12** para trazer a consola de depurg.</span><span class="sxs-lookup"><span data-stu-id="76244-112">Press **F12** to bring up the debug console.</span></span>
    - <span data-ttu-id="76244-113">Tente reproduzir a transação e reveja a mensagem da consola.</span><span class="sxs-lookup"><span data-stu-id="76244-113">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="76244-114">Uma violação do CORS produz um erro de consola sobre a origem.</span><span class="sxs-lookup"><span data-stu-id="76244-114">A CORS violation produces a console error about origin.</span></span>
    - <span data-ttu-id="76244-115">Alguns problemas do CORS não podem ser resolvidos, como quando a sua aplicação redireciona para login.microsoft.com para autenticar, e o token de acesso expira.</span><span class="sxs-lookup"><span data-stu-id="76244-115">Some CORS issues can't be resolved, such as when your app redirects to login.microsoft.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="76244-116">A chamada do CORS falha.</span><span class="sxs-lookup"><span data-stu-id="76244-116">The CORS call then fails.</span></span> <span data-ttu-id="76244-117">Uma solução alternativa para este cenário é prolongar a vida útil do token de acesso, para evitar que expire durante a sessão do utilizador.</span><span class="sxs-lookup"><span data-stu-id="76244-117">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="76244-118">Para obter mais informações sobre como fazê-lo, consulte [as vidas de token configurantes na plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="76244-118">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
4. <span data-ttu-id="76244-119">**Resolução de problemas com base em Snião única**: recomendamos verificar [problemas de sessão em aplicações configuradas com base em SEML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar as soluções para os problemas que você é mais provável encontrar.</span><span class="sxs-lookup"><span data-stu-id="76244-119">**Troubleshooting SAML-based single sign-on**: we recommend checking [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), to find the solutions to the issues you are most likely to encounter.</span></span>
5. <span data-ttu-id="76244-120">**Resolução de problemas com base numa única sessão de registo baseada em palavras-passe:** recomendamos verificar o [único sinal de resolução de palavras-passe baseado em Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar as soluções para os problemas que é mais provável encontrar.</span><span class="sxs-lookup"><span data-stu-id="76244-120">**Troubleshooting password-based single sign-on**: we recommend checking [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), to find the solutions to the issues you are most likely to encounter.</span></span>
6. <span data-ttu-id="76244-121">Para problemas de ligação durante a utilização de uma VPN, consulte [Como utilizar um único sinal (SSO) sobre ligações VPN e Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).</span><span class="sxs-lookup"><span data-stu-id="76244-121">For connection issues while using a VPN, see [How to use single sign on (SSO) over VPN and Wi-Fi connections](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).</span></span>