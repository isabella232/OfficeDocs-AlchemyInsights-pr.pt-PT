---
title: Problemas com base em problemas de assinatura sem emenda sem emenda (SSO)
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
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714883"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Problemas com base em problemas de assinatura sem emenda sem emenda (SSO)

Para conhecer os fundamentos do SSO baseado em palavras-passe, consulte [a autenticação baseada em passwords com o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurar SSO baseado em palavras-passe**

1. [Configure o único sign-on baseado em palavra-passe](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Este artigo entra em mais detalhes sobre a opção SSO baseada em palavra-passe. Se a aplicação que está a adicionar necessitar de configuração personalizada e precisar de utilizar SSO baseado em palavra-passe, então este artigo é para si.
2. [Configure um único sinal baseado em palavra-passe para aplicações on-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - O Application Proxy suporta vários modos de entrada única. O sign-on baseado em palavra-passe destina-se a aplicações que utilizem uma combinação de nome de utilizador/palavra-passe para autenticação. Ao configurar o sign-on baseado em palavra-passe para a sua aplicação, os seus utilizadores têm de iniciar sação na aplicação no local uma vez. Depois disso, o Azure Ative Directory armazena as informações de entrada e fornece-as automaticamente à aplicação quando os seus utilizadores acedem remotamente à sua aplicação.
    - Já devia ter publicado e testado a sua aplicação com o Application Proxy. Caso contrário, siga os passos nas [aplicações de publicação utilizando o Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e, em seguida, continue a sua configuração de SSO baseado em palavra-passe para aplicações on-prem.

Para resolver problemas com sSO baseado em palavras-passe, consulte [o sign-on único baseado em resolução de palavras-passe em Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
