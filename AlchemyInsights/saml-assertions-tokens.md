---
title: Afirmações SAML (Tokens)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885672"
---
# <a name="saml-assertions-tokens"></a>Afirmações SAML (Tokens)

1. As fichas de markup language (SAML) de afirmações de segurança são representações XML de sinistros. Por padrão, os tokens SAML Windows Communication Foundation (WCF) utilizam em cenários de segurança federados são emitidos tokens. Para mais informações, consulte [a SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. A plataforma de identidade da Microsoft emite vários tipos de fichas de segurança no processamento de cada fluxo de autenticação. [A referência de alegações de fichas SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descreve o formato, características de segurança e conteúdo de fichas SAML 2.0.
3. Siga as orientações em [vidas de token configurantes na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para entender como configurar vidas simbólicas.
4. Siga os passos descritos [neste artigo](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) para entender como configurar a encriptação simbólica Azure AD SAML.
5. No Azure AD, pode configurar opções de assinatura de certificado e o algoritmo de assinatura de certificado. Para mais informações, consulte [opções avançadas de assinatura de certificados no token SAML para aplicações de galeria no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
