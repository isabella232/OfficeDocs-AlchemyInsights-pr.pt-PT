---
title: Problemas com base em problemas sem emenda sem emenda (SSO)
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
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747127"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Problemas com base em problemas sem emenda sem emenda (SSO)

- Para aprender a adicionar uma aplicação baseada em OIDC ao seu inquilino Azure, consulte [Quickstart: Crie um único sign-on (SSO) baseado no OIDC para uma aplicação no seu inquilino Azure Ative Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Para obter mais detalhes sobre apps que utilizam a norma OpenID Connect para implementar um único sinal de sípido, consulte [o sign-on único baseado em OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Para obter informações no caso de optar por escrever o seu código enviando e manuseando diretamente pedidos HTTP ou utilizar uma biblioteca de código aberto de terceiros, em vez de utilizar uma das nossas bibliotecas de código aberto, consulte [os protocolos OAuth 2.0 e OpenID Connect na plataforma de identidade Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)

**Protocolos**

1. [Plataforma de identidade da Microsoft e fluxo de subvenção implícito](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) - A característica determinante da concessão implícita é que os tokens (fichas de ID ou fichas de acesso) são devolvidos diretamente do ponto final /autorizado em vez do ponto final /token. Isto é frequentemente utilizado como parte do fluxo de código de autorização, no que é chamado de **"fluxo híbrido" - recuperando o token de ID no pedido /autorizado juntamente com um código de autorização**. Este artigo descreve como programar diretamente contra o protocolo na sua aplicação para solicitar fichas da Azure AD.
2. [Plataforma de identidade da Microsoft e fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - A bolsa de código de autorização OAuth 2.0 pode ser usada em aplicações que são instaladas num dispositivo para ter acesso a recursos protegidos, como APIs web. Utilizando a implementação da plataforma de identidade microsoft de OAuth 2.0, pode **adicionar acesso de iniciar sismo e API às suas aplicações móveis e desktop.** Este artigo descreve como programar diretamente contra o protocolo na sua aplicação usando qualquer idioma.
3. [Plataforma de identidade da Microsoft e protocolo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Quando utilizar a implementação da plataforma de identidade microsoft do OpenID Connect, pode adicionar acesso de s-in e API às suas apps. Este artigo mostra como fazê-lo independentemente da linguagem e descreve como **enviar e receber mensagens HTTP sem utilizar quaisquer bibliotecas de código aberto da Microsoft.**
4. Plataforma de identidade da Microsoft e fluxo de [credenciais de cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Pode utilizar a concessão de credenciais de cliente OAuth 2.0 especificada no RFC 6749, por vezes chamado **OAuth de duas pernas,** para aceder a recursos hospedados na Web utilizando a identidade de uma aplicação. Este tipo de concessão é comumente usado para interações servidor-a-servidor que devem ser executadas em segundo plano, sem interação imediata com um utilizador. Este tipo de aplicações são muitas vezes referidas como **daemons** ou **contas de serviço.** Este artigo descreve como programar diretamente contra o protocolo na sua aplicação.
