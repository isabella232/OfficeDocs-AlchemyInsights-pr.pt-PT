---
title: Asserções SAML (Tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109251"
---
# <a name="saml-assertions-tokens"></a>Asserções SAML (Tokens)

1. Os tokens de Linguagem de Marcação de Segurança (SAML) são representações de afirmações XML. Por predefinição, os tokens SAML Windows Communication Foundation (WCF) utilizados em cenários de segurança federados são emitidos tokens. Para obter mais informações, consulte [Tokens e Afirmações de SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. A plataforma de identidades da Microsoft emite vários tipos de tokens de segurança no processamento de cada fluxo de autenticação. A referência [de afirmações de tokens SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descreve o formato, as características de segurança e os conteúdos de tokens SAML 2.0.
3. Siga as orientações em [Duração de token configurável no plataforma de identidades da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para compreender como configurar as permissões de tokens.
4. Siga os passos neste [](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) artigo para compreender como configurar a encriptação de tokens do Azure AD SAML.
5. No Azure AD, pode configurar as opções de assinatura de certificados e o algoritmo de assinatura de certificados. Para obter mais informações, consulte Opções avançadas de assinatura de certificados no [token SAML para aplicações da galeria Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
