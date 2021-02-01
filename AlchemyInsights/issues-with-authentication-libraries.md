---
title: Problemas com bibliotecas de autenticação
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063641"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="5f212-102">Problemas com bibliotecas de autenticação</span><span class="sxs-lookup"><span data-stu-id="5f212-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="5f212-103">[As bibliotecas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) de autenticação da plataforma de identidade da Microsoft listam bibliotecas de clientes e middleware suportadas pela Microsoft e compatíveis.</span><span class="sxs-lookup"><span data-stu-id="5f212-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="5f212-104">A Microsoft Authentication Library (MSAL) suporta vários [fluxos de autenticação](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) para utilização em diferentes cenários de aplicação.</span><span class="sxs-lookup"><span data-stu-id="5f212-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="5f212-105">Para autenticar e adquirir fichas, inicializa uma nova aplicação de cliente pública ou confidencial no seu código.</span><span class="sxs-lookup"><span data-stu-id="5f212-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="5f212-106">Pode definir várias opções de configuração quando rubricar a aplicação do cliente na Biblioteca de Autenticação do Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="5f212-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="5f212-107">Para saber mais, consulte [as opções de configuração de aplicação](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="5f212-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="5f212-108">**Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="5f212-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="5f212-109">**A partir de 30 de junho de 2020,** deixaremos de adicionar novidades ao ADAL e ao Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="5f212-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="5f212-110">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="5f212-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="5f212-111">**A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="5f212-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="5f212-112">As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não *receberão qualquer suporte técnico ou atualizações de segurança.*</span><span class="sxs-lookup"><span data-stu-id="5f212-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="5f212-113">As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="5f212-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="5f212-114">**Migração ADAL**</span><span class="sxs-lookup"><span data-stu-id="5f212-114">**ADAL Migration**</span></span>

<span data-ttu-id="5f212-115">Recomendamos que atualize para a [Biblioteca de Autenticação da Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tem as funcionalidades e atualizações de segurança mais recentes.</span><span class="sxs-lookup"><span data-stu-id="5f212-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="5f212-116">Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas aplicações para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará das melhorias de segurança e funcionalidades em curso da MSAL.</span><span class="sxs-lookup"><span data-stu-id="5f212-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="5f212-117">Para mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="5f212-117">For more information, see:</span></span>

1. [<span data-ttu-id="5f212-118">Consulte as FAQ da ADAL</span><span class="sxs-lookup"><span data-stu-id="5f212-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="5f212-119">Saiba mais sobre como migrar aplicações por plataforma</span><span class="sxs-lookup"><span data-stu-id="5f212-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="5f212-120">Se precisar de ajuda para entender quais das suas aplicações usam ADAL, recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="5f212-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="5f212-121">O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações de ADAL no seu inquilino que não sejam da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f212-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="5f212-122">**Migração do AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="5f212-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="5f212-123">Para aplicações que estão a usar o Azure AD Graph, siga as nossas orientações para [migrar aplicações AD AD para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="5f212-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="5f212-124">A nossa lista de verificação de migração fornece um ponto de partida.</span><span class="sxs-lookup"><span data-stu-id="5f212-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="5f212-125">O portal de registo da sua aplicação Azure mostra as aplicações que estão a utilizar o AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="5f212-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="5f212-126">Recomendamos que consulte todos os códigos de origem das aplicações e, se aplicável, contacte os ISVs ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="5f212-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="5f212-127">O suporte da Microsoft também pode fornecer-lhe uma lista de todos os usos de gráficos AAD no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="5f212-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="5f212-128">Para que a sua aplicação aceda a dados no Microsoft Graph, o utilizador ou administrador deve conceder-lhe as permissões corretas através de um processo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="5f212-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="5f212-129">As [permissões de referência do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listam as permissões associadas a cada conjunto principal de APIs do Gráfico microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f212-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="5f212-130">Também fornece orientações sobre como usar as permissões.</span><span class="sxs-lookup"><span data-stu-id="5f212-130">It also provides guidance about how to use the permissions.</span></span>
