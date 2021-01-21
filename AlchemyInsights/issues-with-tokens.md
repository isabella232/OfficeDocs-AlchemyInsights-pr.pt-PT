---
title: Problemas com fichas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917037"
---
# <a name="issues-with-tokens"></a>Problemas com fichas

Para gerir questões relacionadas com fichas, pode executar os seguintes passos:

1. Pode especificar o tempo de vida útil de um token de acesso, ID ou SAML emitido pela plataforma de identidade Microsoft. Você pode definir vidas simbólicas para todas as aplicações da sua organização, para uma aplicação multi-inquilina (multi-organização) ou para um diretor de serviço específico na sua organização. Para obter mais informações, consulte [as vidas de símbolos configurais na plataforma de identidade da Microsoft (pré-visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Os tokens de acesso permitem aos clientes ligar de forma segura para as APIs da web protegidas, e são usados por APIs web para realizar autenticação e autorização. De acordo com a especificação OAuth, os tokens de acesso são cordas opacas sem um formato definido - alguns fornecedores de identidade (IDPs) usam GUIDs, outros usam bolhas encriptadas. A plataforma de identidade da Microsoft utiliza uma variedade de formatos de token de acesso, dependendo da configuração da API que aceita o token. Para saber como a sua API pode validar e utilizar as reclamações dentro de um token de acesso, consulte [os tokens de acesso da plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)
3. A Microsoft Authentication Library (MSAL) suporta vários fluxos de autenticação para utilização em diferentes cenários de aplicação. Para mais informações, consulte [os fluxos de autenticação.](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)
4. A bolsa de código de autorização OAuth 2.0 pode ser usada em aplicações que são instaladas num dispositivo para ter acesso a recursos protegidos, como APIs web. Utilizando a implementação da plataforma de identidade microsoft de OAuth 2.0, pode adicionar acesso de s-in e API às suas aplicações móveis e desktop. Consulte [a plataforma de identidade da Microsoft e o fluxo de código de autorização OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) para saber como programar diretamente contra o protocolo na sua aplicação, utilizando qualquer idioma.
5. OpenID Connect (OIDC) é um protocolo de autenticação construído no OAuth 2.0 que pode utilizar para assinar de forma segura num utilizador para uma aplicação. Quando utilizar a implementação do OpenID Connect na plataforma de identidade da Microsoft, pode adicionar acesso de s-in e API às suas apps. [A plataforma de identidade da Microsoft e o protocolo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) mostram como fazê-lo independentemente do idioma e descreve como enviar e receber mensagens HTTP sem utilizar quaisquer bibliotecas de código aberto da Microsoft.
    - O ponto final do UserInfo faz parte da norma OIDC, concebida para devolver reclamações sobre o utilizador que autenticou. Para obter mais informações, consulte o [ponto final da plataforma de identidade da Microsoft UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - A [chamada de uma API web numa aplicação web utilizando a amostra Azure AD e OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) mostra como construir uma aplicação web MVC que usa Azure AD para iniciar sposição usando o protocolo OpenID Connect e, em seguida, ligar para uma API web sob a identidade do utilizador assinado usando fichas obtidas via OAuth 2.0. Esta amostra utiliza o middleware OpenID Connect ASP .Net OWIN e o ADAL .Net.
6. [Configure uma aplicação para expor uma API web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - Neste arranque rápido, regista-se uma API web com a plataforma de identidade da Microsoft e expõe-a a aplicações de clientes adicionando um exemplo de âmbito. Ao registar a sua API web e expô-la através de âmbitos, pode fornecer acesso baseado em permissões aos seus recursos a utilizadores autorizados e aplicações de clientes que acedam à sua API.
7. No Azure Ative Directory B2C (Azure AD B2C), o fluxo de credenciais de senha do proprietário do recurso (ROPC) é um fluxo de autenticação padrão OAuth. Neste fluxo, uma aplicação, também conhecida como a parte dependente, troca credenciais válidas por fichas. As credenciais incluem um ID do utilizador e uma senha. Os tokens devolvidos são um símbolo de identificação, ficha de acesso e um token refrescante. Para obter mais informações, consulte [Configurar um fluxo de credenciais de senha do proprietário de recursos no Azure Ative Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

