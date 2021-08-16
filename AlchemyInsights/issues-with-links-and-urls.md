---
title: Problemas com ligações e URLs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054809"
---
# <a name="issues-with-links-and-urls"></a>Problemas com ligações e URLs

O URI de redirecionamento / URLs de resposta (as duas expressões são permutáveis) são os URLs utilizados pela plataforma de identidade da Microsoft para devolver tokens requisitados da aplicação. Para mais informações sobre estes URLs, consulte os seguintes artigos:

- [Fluxos de autenticação e cenários de aplicação](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Informação sobre como redirecionar os URIs na página **Registo de aplicação** para cada cenário.
- [Restrições e limitações do URI de redirecionamento/URL de resposta](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Não sei como registar o URI de redirecionamento / URL de resposta correto para a minha aplicação**

Quando iniciar sessão com a aplicação que está a desenvolver, se a caixa de diálogo de início de sessão apresentar a mensagem (em inglês) **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, terá de adicionar ao registo da aplicação o URI de redirecionamento que o seu código utilizou no pedido de token para a plataforma de identidades da Microsoft.

Para adicionar um URL de resposta, aceda ao separador **Autenticação** na sua página de **registo da aplicação** no portal do Azure e adicione uma entrada na secção **URIs de Redirecionamento**. O valor que tem de introduzir depende do tipo de aplicação que está a desenvolver, conforme descrito abaixo:

- No caso de aplicações de página única e aplicações web, o URL de resposta é um URL na sua aplicação. Consulte o artigo [Registo de aplicações de página única](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ou [Registar uma aplicação Web com o portal do Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Para as aplicações de ambiente de trabalho, o valor que tem de escolher depende:
    - da plataforma (o MacOS é diferente do Windows ou Linux)
    - da forma como adquire o token (interativamente, através do fluxo do código do dispositivo, da Autenticação Integrada do Windows [IWA] ou através do nome de utilizador/palavra-passe).
    Para obter detalhes, consulte [Aplicações de ambiente de trabalho - Registo de aplicações - URI de Redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Nas aplicações para dispositivos móveis, o URI de redirecionamento depende:
    - da plataforma (iOS/Android/UWP)
    - das informações utilizadas para criar a sua aplicação, como o ID do pacote no iOS, e o nome do pacote e o hash da assinatura no Android. O registo da aplicação no portal do Azure irá ajudá-lo. Para mais informações, consulte [Configuração da plataforma e URIs de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> As APIs Web e algumas das formas silenciosas de adquirir tokens (IWA e nome de utilizador/palavra-passe) não requerem um URI de redirecionamento.

**Implementei a minha aplicação Web e quando estou a testar a aplicação implementada, obtenho uma mensagem sobre um erro de correspondência de um URL de resposta**

Adicione URIs de redirecionamento para todas as localizações nas quais está a implementar a sua aplicação Web. Para mais informações, consulte [Registar uma aplicação Web através do portal do Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Adicione o URI de redirecionamento a uma localização imediatamente após implementar a aplicação nessa localização.

**Não consigo registar URLs de resposta suficientes**

É um ISV e tem um ou vários URIs de redirecionamento para todos os seus clientes. Quer migrar do ADAL/Azure AD v1.0 para o MSAL/a plataforma de identidades da Microsoft e atingiu o [número máximo de URIs de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Para resolver esta situação, [adicione URIs de redirecionamento aos principais de serviço](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) que correspondam a cada um dos seus clientes.
