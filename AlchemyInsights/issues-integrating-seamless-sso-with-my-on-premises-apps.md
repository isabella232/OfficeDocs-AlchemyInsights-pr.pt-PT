---
title: Problemas com a integração de um SSO integrado com as minhas aplicações no local
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028303"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemas com a integração de um SSO integrado com as minhas aplicações no local

Para lidar com problemas de integração do SSO Sem Complicações com aplicações no local, faça o seguinte:

**Passos recomendados**

1. Para configurar uma aplicação no local para o primeiro registo através do **Application Proxy,** consulte Cofre de **palavras-passe** para o acesso único com o [Proxy de Aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. Remoção de problemas do **Proxy** da Aplicação: recomendamos que comece a rever o fluxo de remoção de problemas, Depurar problemas do [Application Proxy Connector,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)para determinar se os conectores do Proxy da Aplicação estão configurados corretamente. Se ainda estiver com problemas de ligação à aplicação, siga os passos de remoção de problemas em Depurar problemas da aplicação [Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)de Aplicação . Pode identificar problemas [de CORS ao](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizar as seguintes ferramentas de depuração do browser:
    1. Inceda o browser e navegue até à aplicação Web.
    1. Prima **F12** para trazer a consola de depuração.
    1. Tente reproduzir a transação e reveja a mensagem da consola. Uma violação CORS produz um erro de consola sobre a origem.
    1. Alguns problemas do CORS não podem ser resolvidos, como quando a sua aplicação redireciona para login.microsoftonline.com para autenticar e o token de acesso expira. A chamada CORS falha. Uma forma de resolver este cenário é prolongar a duração do token de acesso para impedir que expire durante a sessão de um utilizador. Para obter mais informações sobre como fazê-lo, consulte o t causador de vida [configurável dos tokens plataforma de identidades da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documentos recomendados**

- [Como configurar o registo único numa aplicação Proxy de Aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML single sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Compreender e resolver problemas Azure Active Directory CORS do Proxy Application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Remoção de configurações de delegação restritas de Kerberos para o Proxy de Aplicações](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)