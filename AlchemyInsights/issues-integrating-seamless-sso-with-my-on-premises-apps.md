---
title: Problemas com a integração do Seamless SSO com as minhas aplicações no local
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868720"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemas com a integração do Seamless SSO com as minhas aplicações no local

Para resolver problemas com a integração do SSO sem emenda com aplicações no local, faça o seguinte:

**Passos recomendados**

1. Para configurar um **pedido no local** para um único sinal de acesso através de **Aplicação Proxy**, consulte [abotoação de palavra-passe para um único sinal de acesso com procuração de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Problemas de resolução de problemas Problemas Aplicações Problemas de procuração**: recomendamos que comece a rever o fluxo de resolução de [problemas, problemas de Conector de Procuração de Aplicações de Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), para determinar se os conectores de procuração de aplicação estão configurados corretamente. Se ainda tiver problemas em ligar-se à aplicação, siga os passos de resolução de problemas em problemas de [aplicação de depuração](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Pode [identificar problemas de CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizando as seguintes ferramentas de depuragem do navegador:
    1. Lance o navegador e navegue para a aplicação web.
    1. Pressione **f12** para trazer a consola de depurg.
    1. Tente reproduzir a transação e reveja a mensagem da consola. Uma violação do CORS produz um erro de consola sobre a origem.
    1. Alguns problemas do CORS não podem ser resolvidos, como quando a sua aplicação redireciona para login.microsoftonline.com para autenticar, e o token de acesso expira. A chamada do CORS falha. Uma solução alternativa para este cenário é prolongar a vida útil do token de acesso, para evitar que expire durante a sessão do utilizador. Para obter mais informações sobre como fazê-lo, consulte [as vidas de token configurantes na plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Documentos recomendados**

- [Como configurar um único sign-on para uma aplicação de procuração de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML único sinal de inscrição para aplicações no local com Proxy de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Compreender e resolver problemas de aplicação de diretório ativo Azure](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Resolução de problemas Kerberos limitou configurações da delegação para aplicação proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)