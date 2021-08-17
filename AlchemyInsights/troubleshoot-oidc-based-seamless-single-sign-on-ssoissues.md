---
title: Remoção de problemas de SSO (SSO) baseados em OIDC
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105789"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Remoção de problemas de SSO (SSO) baseados em OIDC

- Para saber como adicionar uma aplicação baseada em OIDC ao seu inquilino do Azure, consulte Guia de Inquilino: Configurar o SSO (SSO) baseado em OIDC para uma aplicação no seu inquilino [do Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Para obter mais detalhes sobre as aplicações que utilizam o OpenID Ligação padrão para implementar o primeiro sinal, consulte Compreender o sinal de utilização única baseado em [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Para obter informações caso opte por escrever o código ao enviar e tratar diretamente dos pedidos HTTP ou utilizar uma biblioteca de open source de terceiros em vez de utilizar uma das nossas bibliotecas de open source, consulte [protocolos OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)e OpenID Ligação no plataforma de identidades da Microsoft.

**Protocolos**

1. fluxo de concessão [plataforma de identidades da Microsoft implícito](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – a característica definitiva da concessão implícita é que os tokens (tokens ID ou tokens de acesso) são devolvidos diretamente a partir do ponto final /authorize em vez do ponto final /token. Isto é frequentemente utilizado como parte do fluxo de código de autorização, no que é denominado "fluxo híbrido" - obter o **token ID no pedido /autorizar** juntamente com um código de autorização . Este artigo descreve como programar diretamente contra o protocolo na sua aplicação para pedir tokens do Azure AD.
2. fluxo de código de autorização plataforma de identidades da Microsoft e [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - A concessão do código de autorização OAuth 2.0 pode ser utilizada em aplicações instaladas num dispositivo para obter acesso a recursos protegidos, como as APIs Web. Com a plataforma de identidades da Microsoft da OAuth 2.0, pode adicionar o acesso de lote e da API às suas aplicações móveis e **de ambiente de trabalho.** Este artigo descreve como programar diretamente contra o protocolo na sua aplicação, utilizando qualquer idioma.
3. [plataforma de identidades da Microsoft e o protocolo OpenID Ligação](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Ao utilizar a implementação do OpenID Ligação da plataforma de identidades da Microsoft, pode adicionar o acesso de entrada e da API às suas aplicações. Este artigo mostra como fazê-lo independentemente do idioma e descreve como enviar e receber mensagens HTTP sem utilizar **bibliotecas de open source da Microsoft.**
4. plataforma de identidades da Microsoft e o fluxo de credenciais de cliente [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Pode utilizar a concessão de credenciais de cliente OAuth 2.0 especificadas em RFC 6749, por vezes denominada **OAuth** de duas leções, para aceder a recursos alojados na Web utilizando a identidade de uma aplicação. Este tipo de concessão é frequentemente utilizado para interações servidor a servidor que têm de ser executada em segundo plano, sem interação imediata com um utilizador. Estes tipos de aplicações são muitas vezes denominados **daemons** ou **contas de serviço.** Este artigo descreve como programar diretamente contra o protocolo na sua aplicação.
