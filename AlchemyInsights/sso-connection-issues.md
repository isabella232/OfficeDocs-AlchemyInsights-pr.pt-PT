---
title: Problemas de Ligação do SSO
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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084357"
---
# <a name="sso-connection-issues"></a>Problemas de Ligação do SSO

1. Siga o [Guia de Instrução Rápida: configurar propriedades de um guia de](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) aplicação para configurar a sua aplicação.
2. Dependendo da aplicação e [da opção de primeiro-dia que](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) escolher, siga as orientações adequadas abaixo:
    - Para configurar  uma aplicação no local para o registo único baseado em **SAML,** consulte o registo único do SAML para aplicações no local com [o Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Para configurar uma aplicação **na nuvem** para o registo único baseado em **palavra-passe,** consulte Configurar o sinal  [de única palavra-passe no](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Para configurar uma aplicação no local para o primeiro registo através do **Application Proxy,** consulte Cofre de **palavras-passe** para o acesso único com o [Proxy de Aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. Remoção de problemas do **Proxy** de Aplicação : recomendamos que comece a rever o fluxo de remoção de problemas, Depurar problemas do [Application Proxy Connector,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)para determinar se as conexões Proxy da Aplicação estão configuradas corretamente. Se continuar a ter problemas em ligar à aplicação, siga o fluxo de remoção de problemas em Depurar problemas da aplicação [Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)do Application . Pode identificar problemas [do CORS através das](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ferramentas de depuração do browser:
    - Inceda o browser e navegue até à aplicação Web.
    - Prima **F12** para trazer a consola de depuração.
    - Tente reproduzir a transação e reveja a mensagem da consola. Uma violação CORS produz um erro de consola sobre a origem.
    - Alguns problemas do CORS não podem ser resolvidos, como quando a sua aplicação redireciona para login.microsoft.com para autenticar e o token de acesso expira. A chamada CORS falha. Uma forma de resolver este cenário é prolongar a duração do token de acesso para impedir que expire durante a sessão de um utilizador. Para obter mais informações sobre como fazê-lo, consulte o t causador de vida [configurável dos tokens plataforma de identidades da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Remoção de problemas de um só fim com base em **SAML:** recomendamos que sele sejam verificados Problemas ao entrar em aplicações configuradas com base em [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)para encontrar as soluções para os problemas que é mais provável que encontre.
5. **Remoção** de problemas de acesso único com base em palavra-passe : recomendamos que verifique a remoção de problemas de o primeiro-lo baseado em [palavra-passe no Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)para encontrar as soluções para os problemas com que provavelmente irá encontrar.
6. Para problemas de ligação ao utilizar uma VPN, consulte Como utilizar o [SSO (single sign on)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)através de VPN e Wi-Fi ligações .
