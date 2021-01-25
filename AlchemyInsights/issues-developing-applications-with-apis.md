---
title: Questões que desenvolvem aplicações com APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975014"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="3da4e-102">Questões que desenvolvem aplicações com APIs</span><span class="sxs-lookup"><span data-stu-id="3da4e-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="3da4e-103">Para começar a utilizar o Azure Ative Directory Graph API, consulte o [guia de arranque rápido Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , ou veja a [documentação de referência interativa AZure AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="3da4e-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="3da4e-104">**Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="3da4e-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="3da4e-105">**A partir de 30 de junho de 2020,** deixaremos de adicionar novidades ao ADAL e ao Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="3da4e-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="3da4e-106">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="3da4e-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="3da4e-107">**A partir de 30 de junho de 2022,** terminaremos o suporte ao ADAL e ao Azure AD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="3da4e-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="3da4e-108">As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não receberão qualquer suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="3da4e-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="3da4e-109">As aplicações que utilizam o Azure AD Graph após este tempo podem deixar de receber respostas do ponto final do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="3da4e-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="3da4e-110">**Migração ADAL**</span><span class="sxs-lookup"><span data-stu-id="3da4e-110">**ADAL Migration**</span></span>

<span data-ttu-id="3da4e-111">Recomendamos a atualização para a Biblioteca de Autenticação da [Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que possui as mais recentes funcionalidades e atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="3da4e-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="3da4e-112">Se estiver a utilizar aplicações da Microsoft, saiba que a Microsoft está em processo de migrar as suas aplicações para o MSAL até ao fim do prazo de suporte, garantindo que beneficiará da segurança contínua da MSAL e das melhorias de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="3da4e-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="3da4e-113">[Leia as FAQ ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="3da4e-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="3da4e-114">[Saiba como migrar aplicações por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="3da4e-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="3da4e-115">Se precisar de ajuda para entender quais das suas aplicações usam ADAL, recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="3da4e-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="3da4e-116">O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações ADAL não-Microsoft no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="3da4e-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="3da4e-117">**Migração de gráficos AAD**</span><span class="sxs-lookup"><span data-stu-id="3da4e-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="3da4e-118">Para aplicações que estão a usar o Azure AD Graph, siga as nossas orientações para migrar [aplicações AD AD para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="3da4e-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="3da4e-119">[A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="3da4e-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="3da4e-120">O portal de registo de aplicações Azure mostra quais as aplicações que estão a utilizar o AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="3da4e-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="3da4e-121">Recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer ISV ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="3da4e-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="3da4e-122">O suporte da Microsoft também pode fornecer-lhe uma lista de todos os usos de gráficos AAD no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="3da4e-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="3da4e-123">Para que a sua aplicação aceda a dados no Microsoft Graph, o utilizador ou administrador deve conceder-lhe as permissões corretas através de um processo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="3da4e-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="3da4e-124">As [permissões de referência do Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) listam as permissões associadas a cada conjunto principal de APIs do Gráfico microsoft.</span><span class="sxs-lookup"><span data-stu-id="3da4e-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="3da4e-125">Também fornece orientações sobre como usar as permissões.</span><span class="sxs-lookup"><span data-stu-id="3da4e-125">It also provides guidance about how to use the permissions.</span></span>
