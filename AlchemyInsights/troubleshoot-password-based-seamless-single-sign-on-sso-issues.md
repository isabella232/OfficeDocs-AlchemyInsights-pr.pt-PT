---
title: Remoção de problemas de SSO (SSO) baseados em Palavras-passe Sem Palavras-passe
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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972835"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Remoção de problemas de SSO (SSO) baseados em Palavras-passe Sem Palavras-passe

Para saber os princípios básicos do SSO baseado em palavra-passe, consulte Autenticação baseada em [palavra-passe com Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurar o SSO baseado em Palavra-passe**

1. [Configurar o acesso único baseado em palavra-passe](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – este artigo vai mais detalhes sobre a opção de SSO baseada em palavra-passe. Se a aplicação que está a adicionar necessitar de configuração personalizada e precisar de utilizar o SSO baseado em palavra-passe, este artigo é para si.
2. [Configurar o registo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) único baseado em palavra-passe para aplicações no prem - O Proxy de Aplicação suporta vários modos de funcionamento único. O estabelecimento com base em palavras-passe destina-se a aplicações que utilizam uma combinação de nome de utilizador/palavra-passe para autenticação. Quando configura o registo com base em palavras-passe para a sua aplicação, os seus utilizadores têm de entrar uma vez na aplicação no local. Depois disso, o Azure Active Directory armazena as informações de inscrição e fornece-as automaticamente à aplicação quando os seus utilizadores acedem às mesmas remotamente.
    - Já deverá ter publicado e testado a sua aplicação com o Application Proxy. Caso não o seja, siga os passos em Publicar aplicações com o [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e, em seguida, continue a configuração do SSO baseado em palavra-passe para aplicações no -prem.

Para remoção de problemas de SSO baseados em palavra-passe, consulte Remoção de problemas de acesso único baseados em [palavra-passe no Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
