---
title: Questões que desenvolvem aplicações
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974771"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="af9ef-102">Questões que desenvolvem aplicações</span><span class="sxs-lookup"><span data-stu-id="af9ef-102">Issues developing applications</span></span>

<span data-ttu-id="af9ef-103">Para resolver os problemas mais comuns ao construir aplicações Azure Ative Directory (AD), consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="af9ef-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="af9ef-104">Estou a ver problemas em iniciar sessão para aplicações usando apenas o navegador Chrome</span><span class="sxs-lookup"><span data-stu-id="af9ef-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="af9ef-105">Não sei como alterar os incumprimentos de toda a vida para a minha aplicação.</span><span class="sxs-lookup"><span data-stu-id="af9ef-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="af9ef-106">Estou confuso sobre como funciona o consentimento da candidatura</span><span class="sxs-lookup"><span data-stu-id="af9ef-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="af9ef-107">Não sei como conceder permissões à minha candidatura.</span><span class="sxs-lookup"><span data-stu-id="af9ef-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="af9ef-108">Não entendo a diferença entre permissões de candidaturas delegadas.</span><span class="sxs-lookup"><span data-stu-id="af9ef-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="af9ef-109">\***Fim do suporte para Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="af9ef-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="af9ef-110">A partir de 30 de junho de 2020, deixaremos de adicionar quaisquer novidades à Azure Ative Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="af9ef-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="af9ef-111">Continuaremos a fornecer suporte técnico e atualizações de segurança, mas deixaremos de fornecer atualizações de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="af9ef-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="af9ef-112">A partir de 30 de junho de 2022, terminaremos o suporte para o ADAL e a AAD Graph e deixaremos de fornecer suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="af9ef-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="af9ef-113">Como resultado desta condição, as seguintes são as implicações:</span><span class="sxs-lookup"><span data-stu-id="af9ef-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="af9ef-114">As aplicações que utilizam o ADAL nas versões de SO existentes continuarão a funcionar após este período, mas não receberão qualquer suporte técnico ou atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="af9ef-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="af9ef-115">As aplicações que utilizam o Gráfico AAD após este tempo podem deixar de receber respostas do ponto final do Gráfico AAD</span><span class="sxs-lookup"><span data-stu-id="af9ef-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="af9ef-116">_ *Migração ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="af9ef-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="af9ef-117">Se estiver a utilizar aplicações da Microsoft, recomendamos a atualização para a Microsoft Authentication Library (MSAL), que tem as mais recentes funcionalidades e atualizações de segurança.</span><span class="sxs-lookup"><span data-stu-id="af9ef-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="af9ef-118">Esta recomendação encontra-se no contexto de a Microsoft iniciar o processo de migração das suas apps para a MSAL até ao fim do prazo de suporte.</span><span class="sxs-lookup"><span data-stu-id="af9ef-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="af9ef-119">A migração pela Microsoft das suas apps para o MSAL garante que as aplicações beneficiam da segurança contínua da MSAL e das melhorias de funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="af9ef-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="af9ef-120">Leia as FAQ ADAL</span><span class="sxs-lookup"><span data-stu-id="af9ef-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="af9ef-121">Saiba como migrar aplicações por plataforma</span><span class="sxs-lookup"><span data-stu-id="af9ef-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="af9ef-122">Se precisar de ajuda para entender qual das suas aplicações usa ODAL, recomendamos que reveja todo o código fonte das suas aplicações e, se for caso disso, contacte quaisquer fornecedores de software independentes (ISV) ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="af9ef-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="af9ef-123">O suporte da Microsoft também pode fornecer-lhe uma lista de todas as aplicações ADAL não-Microsoft no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="af9ef-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="af9ef-124">**Migração de gráficos AAD**</span><span class="sxs-lookup"><span data-stu-id="af9ef-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="af9ef-125">Para aplicações que estão a usar o AAD Graph, siga a nossa orientação para migrar aplicações AAD Graph para o Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="af9ef-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="af9ef-126">[A nossa lista de verificação de migração fornece um ponto de partida.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="af9ef-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="af9ef-127">O portal de registo de aplicações Azure mostra quais as aplicações que estão a utilizar o AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="af9ef-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="af9ef-128">Recomendamos que reveja todo o código fonte das suas aplicações e, se aplicável, contacte quaisquer fornecedores de software independentes (ISV) ou fornecedores de aplicações.</span><span class="sxs-lookup"><span data-stu-id="af9ef-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="af9ef-129">O suporte da Microsoft também pode fornecer-lhe informações sobre o uso do AAD Graph no seu inquilino.</span><span class="sxs-lookup"><span data-stu-id="af9ef-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







