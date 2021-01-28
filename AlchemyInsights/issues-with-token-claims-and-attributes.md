---
title: Problemas com reclamações e atributos token
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035969"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="9d222-102">Problemas com reclamações e atributos token</span><span class="sxs-lookup"><span data-stu-id="9d222-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="9d222-103">**Atualizar, configurar ou remover reclamações simbólicas**</span><span class="sxs-lookup"><span data-stu-id="9d222-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="9d222-104">Ao utilizar o Azure Ative Directory (Azure AD), pode [personalizar o tipo de reclamação para a reivindicação de funções](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) no token de resposta que recebe depois de autorizar uma aplicação.</span><span class="sxs-lookup"><span data-stu-id="9d222-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="9d222-105">Os desenvolvedores de aplicações podem usar reclamações opcionais nas suas aplicações AZure AD para especificar quais as alegações que pretendem em fichas enviadas para a sua aplicação.</span><span class="sxs-lookup"><span data-stu-id="9d222-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="9d222-106">Para obter mais informações, consulte [Fornecer reclamações opcionais à sua aplicação.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="9d222-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="9d222-107">[Configure pedidos de pedidos de candidaturas com a Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="9d222-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="9d222-108">Se utilizar o 'Sign-on' único sem emenda na sua aplicação, consulte [as reclamações personalizadas emitidas no token SAML para aplicações empresariais](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="9d222-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="9d222-109">**Mapeamento de atributos de reclamações**</span><span class="sxs-lookup"><span data-stu-id="9d222-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="9d222-110">Para configurar a política de mapeamento de reclamações utilizando o PowerShell, consulte [Personalizar reclamações emitidas em fichas para uma aplicação específica num inquilino (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="9d222-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="9d222-111">Os atributos de extensão de esquema de diretório fornecem uma forma de armazenar dados adicionais no Azure Ative Directory em objetos de utilizador e outros objetos de diretório, tais como grupos, detalhes do inquilino, diretores de serviço.</span><span class="sxs-lookup"><span data-stu-id="9d222-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="9d222-112">Apenas os atributos de extensão em objetos do utilizador podem ser usados para emitir reclamações para aplicações.</span><span class="sxs-lookup"><span data-stu-id="9d222-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="9d222-113">[A utilização de atributos de extensão de esquema de diretório em sinistros](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) descreve como utilizar atributos de extensão de esquema de diretório para enviar dados do utilizador para aplicações em alegações simbólicas.</span><span class="sxs-lookup"><span data-stu-id="9d222-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="9d222-114">Para obter mais informações sobre sinistros simbólicos, consulte:</span><span class="sxs-lookup"><span data-stu-id="9d222-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="9d222-115">Reclamações em fichas de acesso</span><span class="sxs-lookup"><span data-stu-id="9d222-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="9d222-116">Reclamações num id_token</span><span class="sxs-lookup"><span data-stu-id="9d222-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="9d222-117">[Reclamações](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que pode esperar em fichas de ID e fichas de acesso emitidas pela Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="9d222-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="9d222-118">Referência de reclamações de ficha SAML</span><span class="sxs-lookup"><span data-stu-id="9d222-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
