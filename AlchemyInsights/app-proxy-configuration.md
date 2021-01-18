---
title: Configuração de procuração de aplicativos
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885524"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="e0217-102">Configuração de procuração de aplicativos</span><span class="sxs-lookup"><span data-stu-id="e0217-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="e0217-103">Para entender como configurar uma aplicação Proxy de aplicação no Azure AD para expor as suas aplicações no local à nuvem, consulte [como configurar uma aplicação Proxy de aplicação.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="e0217-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="e0217-104">O único sinal de sso permite aos seus utilizadores aceder a uma aplicação sem autenticar várias vezes.</span><span class="sxs-lookup"><span data-stu-id="e0217-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="e0217-105">Permite que a autenticação única ocorra na nuvem, contra o Azure Ative Directory, e permite que o serviço ou Conector personiem o utilizador para completar quaisquer desafios adicionais de autenticação da aplicação.</span><span class="sxs-lookup"><span data-stu-id="e0217-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="e0217-106">Para saber mais, consulte [Como configurar um único sinal de inscrição para uma aplicação de Procuração de Aplicação.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="e0217-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="e0217-107">Use [este artigo](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) para resolver problemas comuns que as pessoas enfrentam ao criar uma nova aplicação de procuração de aplicações.</span><span class="sxs-lookup"><span data-stu-id="e0217-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="e0217-108">Se tiver algum problema em configurar a autenticação de back-end para a sua aplicação, poderá necessitar de [configurações de delegação restritas de Kerberos para aplicação proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ou seguir orientações sobre [configurar a aplicação com o PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) para resolver o seu problema.</span><span class="sxs-lookup"><span data-stu-id="e0217-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
