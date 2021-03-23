---
title: Trabalhar com bibliotecas de autenticação
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036872"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="378c0-102">Trabalhar com bibliotecas de autenticação</span><span class="sxs-lookup"><span data-stu-id="378c0-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="378c0-103">Para resolver o problema da Biblioteca de Autenticação do Microsoft (MSAL), execute os seguintes passos recomendados:</span><span class="sxs-lookup"><span data-stu-id="378c0-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="378c0-104">**Trabalhar com a MSAL**: [Bibliotecas de autenticação da plataforma de identidade microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - Este artigo mostra o suporte da Microsoft Authentication Library para vários tipos de aplicações.</span><span class="sxs-lookup"><span data-stu-id="378c0-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="378c0-105">Inclui links para código fonte de biblioteca; onde obter o pacote para o projeto da sua aplicação; e se a biblioteca suporta o acesso ao utilizador (autenticação), o acesso a APIs web protegidas (autorização), ou ambos.</span><span class="sxs-lookup"><span data-stu-id="378c0-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="378c0-106">**Resolução de problemas Autenticação**: O MSAL suporta vários fluxos de autenticação para utilização em diferentes cenários de aplicação.</span><span class="sxs-lookup"><span data-stu-id="378c0-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="378c0-107">Dependendo da forma como a aplicação do seu cliente é construída, o MSAL pode utilizar um ou mais dos fluxos de autenticação suportados pela plataforma de identidade microsoft.</span><span class="sxs-lookup"><span data-stu-id="378c0-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="378c0-108">Estes fluxos podem produzir vários tipos de fichas e códigos de autorização, e requerem diferentes fichas para fazê-los funcionar.</span><span class="sxs-lookup"><span data-stu-id="378c0-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="378c0-109">**Tokens de acesso**: [Fichas de acesso à plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Saiba como a sua API pode validar e utilizar as reclamações dentro de um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="378c0-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="378c0-110">Toda a documentação deste artigo, exceto quando anotado, aplica-se apenas a fichas emitidas para APIs que tenha registado.</span><span class="sxs-lookup"><span data-stu-id="378c0-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="378c0-111">Não se aplica a fichas emitidas para APIs detidas pela Microsoft, nem esses tokens podem ser usados para validar como a plataforma de identidade da Microsoft emitirá fichas para uma API que cria.</span><span class="sxs-lookup"><span data-stu-id="378c0-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="378c0-112">**Fim do suporte para a Biblioteca de Autenticação do Diretório Ativo Azure (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="378c0-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="378c0-113">**A partir de 30 de junho de 2020,** deixaremos de adicionar novas funcionalidades ao ADAL e ao Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="378c0-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="378c0-114">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="378c0-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="378c0-115">**A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="378c0-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="378c0-116">As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não *receberão qualquer suporte técnico ou atualizações de segurança.*</span><span class="sxs-lookup"><span data-stu-id="378c0-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="378c0-117">As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="378c0-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="378c0-118">**Migração ADAL**</span><span class="sxs-lookup"><span data-stu-id="378c0-118">**ADAL Migration**</span></span>

- <span data-ttu-id="378c0-119">Recomendamos a atualização ao MSAL, que tem as mais recentes funcionalidades e atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="378c0-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="378c0-120">Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas apps para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará da segurança contínua da MSAL e das melhorias de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="378c0-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="378c0-121">[Leia as FAQ ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="378c0-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="378c0-122">[Saiba como migrar aplicações por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="378c0-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="378c0-123">Se, depois de ler o guia para a plataforma da sua aplicação, tiver perguntas adicionais, pode publicar no [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) com a etiqueta [azure-ad-adal-depreciação] ou abrir um problema no repositório GitHub da biblioteca.</span><span class="sxs-lookup"><span data-stu-id="378c0-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="378c0-124">Consulte a secção [de Línguas e Quadros](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) do artigo **de visão geral** do MSAL para obter links para o repo de cada biblioteca.</span><span class="sxs-lookup"><span data-stu-id="378c0-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="378c0-125">**Se precisar de ajuda para entender quais das suas aplicações usam ADAL,** recomendamos que reveja todo o código fonte das suas apps.</span><span class="sxs-lookup"><span data-stu-id="378c0-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="378c0-126">Se aplicável, contacte qualquer fornecedor de software independente (ISVs) ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="378c0-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="378c0-127">O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="378c0-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







