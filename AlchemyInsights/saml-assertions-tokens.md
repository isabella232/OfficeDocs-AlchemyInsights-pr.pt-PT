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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="b7089-102">Afirmações SAML (Tokens)</span><span class="sxs-lookup"><span data-stu-id="b7089-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="b7089-103">As fichas de markup language (SAML) de afirmações de segurança são representações XML de sinistros.</span><span class="sxs-lookup"><span data-stu-id="b7089-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="b7089-104">Por padrão, os tokens SAML Windows Communication Foundation (WCF) utilizam em cenários de segurança federados são emitidos tokens.</span><span class="sxs-lookup"><span data-stu-id="b7089-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="b7089-105">Para mais informações, consulte [a SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="b7089-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="b7089-106">A plataforma de identidade da Microsoft emite vários tipos de fichas de segurança no processamento de cada fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b7089-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="b7089-107">[A referência de alegações de fichas SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descreve o formato, características de segurança e conteúdo de fichas SAML 2.0.</span><span class="sxs-lookup"><span data-stu-id="b7089-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="b7089-108">Siga as orientações em [vidas de token configurantes na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para entender como configurar vidas simbólicas.</span><span class="sxs-lookup"><span data-stu-id="b7089-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="b7089-109">Siga os passos descritos [neste artigo](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) para entender como configurar a encriptação simbólica Azure AD SAML.</span><span class="sxs-lookup"><span data-stu-id="b7089-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="b7089-110">No Azure AD, pode configurar opções de assinatura de certificado e o algoritmo de assinatura de certificado.</span><span class="sxs-lookup"><span data-stu-id="b7089-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="b7089-111">Para mais informações, consulte [opções avançadas de assinatura de certificados no token SAML para aplicações de galeria no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="b7089-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
