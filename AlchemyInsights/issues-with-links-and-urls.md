---
title: Problemas com links e URLs
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974750"
---
# <a name="issues-with-links-and-urls"></a>Problemas com links e URLs

Redirecionar URLs URI/resposta (ambas as expressões são permutáveis) são os URLs utilizados pela plataforma de identidade da Microsoft para devolver fichas solicitadas pela aplicação. Para obter informações sobre estes URLs, consulte os seguintes artigos:

- [Fluxos de autenticação e cenários de aplicação](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Informação sobre os URIs redirecionados na página **de registo** da App para cada cenário.
- [Redirecionar restrições e limitações de URL URI/resposta](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Não sei como registar o URI de redirecionamento certo / URL de resposta para a minha app**

Quando iniciar seduca com a aplicação que está a desenvolver, se o diálogo de inscrição apresentar **AADSTS50011: O url <your app ID> de resposta especificado no pedido não corresponde aos urls de resposta configurados para a aplicação,** terá de adicionar ao seu registo de candidatura, o URI de redirecionamento que o seu código utilizou no pedido simbólico para a plataforma de identidade da Microsoft.

Para adicionar um URL de resposta, aceda ao separador **Autenticação** na página **de registo** da sua candidatura no portal Azure e adicione uma entrada na secção **URIs redirecionado.** Os URIs de redirecionamento são dactilografados (Web ou mobile/desktop). O valor que precisa de introduzir depende do tipo de aplicação que está a construir, conforme descrito abaixo:

- Para aplicações de uma página única e aplicações web, o URL de resposta é um URL na sua aplicação. Ver [registo de aplicações de página única](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ou registar uma [aplicação web utilizando o portal Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Para aplicações de ambiente de trabalho, o valor que precisa de escolher depende de:
    - a plataforma (MacOS é diferente do Windows ou Linux)
    - a forma como adquire o token (interativamente, com fluxo de código do dispositivo, com autenticação integrada do Windows [IWA] ou com nome de utilizador/senha).
    Para mais detalhes, consulte [aplicações de Desktop - Registo de aplicações - Redirecionar uRi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Para aplicações móveis, o URI de redirecionamento depende de:
    - a plataforma (iOS/Android/UWP)
    - as informações utilizadas para construir a sua app, como o bundle ID no iOS, e o nome do pacote e hash de assinatura no Android O registo de aplicações do portal Azure irão ajudá-lo. Para mais detalhes, consulte [a configuração da plataforma e redirecione uris](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> As APIs web e algumas das formas silenciosas de adquirir fichas (IWA e username/password) não requerem um URI de redirecionamento.

**Implementei a minha aplicação web e quando testei a aplicação implementada, recebo uma mensagem de incompatibilidade de url de resposta**

Adicione URIs de redirecionamento para todas as localizações em que está a implementar a sua aplicação web. Para obter mais informações, consulte [Registar uma aplicação web utilizando o portal Azure.](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)

> [!NOTE]
> Adicione o URI de redirecionamento para uma localização imediatamente após ter implantado a aplicação naquele local.

**Não consigo registar URLs de resposta suficientes.**

Você é um ISV e tem um ou vários URIs redirecionados para cada cliente seu. Pretende migrar de ADAL/Azure AD v1.0 para MSAL/a plataforma de identidade microsoft e atingir o [número máximo de URIs de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Para resolver isto, [adicione URIs redirecionando para os principais de serviço](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) que correspondem a cada um dos seus clientes.
