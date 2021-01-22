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
# <a name="sso-connection-issues"></a>Problemas de conexão SSO

1. Siga o [Quickstart: Configure propriedades para um](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guia de aplicações para configurar a sua aplicação.
2. Dependendo da aplicação e da [opção de inscrição única](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) que escolheu, siga as orientações apropriadas abaixo:
    - Para configurar um pedido no local para um único **sign-on** **baseado em SAML,** consulte [a SAML single-sign-on para aplicações no local com Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Para configurar uma **aplicação** em nuvem para **um único sinal de assinatura baseado em palavra-passe,** consulte  [configurar a palavra-passe de um único sinal](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Para configurar um **pedido no local** para um único sinal de acesso através de **Aplicação Proxy**, consulte [abotoação de palavra-passe para um único sinal de acesso com procuração de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Problemas de resolução de problemas Problemas Aplicação Problemas de procuração**: recomendamos que comece a rever o fluxo de resolução [de problemas, problemas de Conector de Procuração de Aplicações de Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), para determinar se os conectores de procuração de aplicação estão configurados corretamente. Se ainda tiver problemas em ligar-se à aplicação, siga o fluxo de resolução de problemas em problemas de [aplicação de depuração](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizando ferramentas de depuragem de navegador:
    - Lance o navegador e navegue para a aplicação web.
    - Pressione **f12** para trazer a consola de depurg.
    - Tente reproduzir a transação e reveja a mensagem da consola. Uma violação do CORS produz um erro de consola sobre a origem.
    - Alguns problemas do CORS não podem ser resolvidos, como quando a sua aplicação redireciona para login.microsoft.com para autenticar, e o token de acesso expira. A chamada do CORS falha. Uma solução alternativa para este cenário é prolongar a vida útil do token de acesso, para evitar que expire durante a sessão do utilizador. Para obter mais informações sobre como fazê-lo, consulte [as vidas de token configurantes na plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Resolução de problemas com base em Snião única**: recomendamos verificar [problemas de sessão em aplicações configuradas com base em SEML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar as soluções para os problemas que você é mais provável encontrar.
5. **Resolução de problemas com base numa única sessão de registo baseada em palavras-passe:** recomendamos verificar o [único sinal de resolução de palavras-passe baseado em Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar as soluções para os problemas que é mais provável encontrar.
6. Para problemas de ligação durante a utilização de uma VPN, consulte [Como utilizar um único sinal (SSO) sobre ligações VPN e Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
