---
title: Problemas de acesso condicional
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014889"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="91c1d-102">Problemas de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="91c1d-102">Conditional access issues</span></span>

<span data-ttu-id="91c1d-103">**Resolver problemas com o Diagnóstico de Inscrição**</span><span class="sxs-lookup"><span data-stu-id="91c1d-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="91c1d-104">Pode rapidamente descobrir o que aconteceu ou diagnosticar problemas relacionados com o s-in do utilizador utilizando o [Diagnóstico de Inscrição:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="91c1d-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="91c1d-105">Lance o Diagnóstico de Inscrição.</span><span class="sxs-lookup"><span data-stu-id="91c1d-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="91c1d-106">Encontre o evento para analisar inserindo nos detalhes que tem sobre o utilizador, aplicação, hora de entrada, Id de pedido ou Id de correlação.</span><span class="sxs-lookup"><span data-stu-id="91c1d-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="91c1d-107">Reveja os resultados de diagnóstico mostrando os detalhes do que aconteceu e que ações pode tomar para fazer alterações (se forem necessárias alterações).</span><span class="sxs-lookup"><span data-stu-id="91c1d-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="91c1d-108">**Passos para resolução de problemas de um 'Sign-In'**</span><span class="sxs-lookup"><span data-stu-id="91c1d-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="91c1d-109">Navegue para a página de inscrição Azure AD.</span><span class="sxs-lookup"><span data-stu-id="91c1d-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="91c1d-110">Filtrar as entradas pelo utilizador, intervalo de tempo, aplicação, estado, aplicação do cliente, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="91c1d-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="91c1d-111">Selecione um evento de inscrição e veja o separador Acesso Condicional para ver quais as políticas que foram avaliadas.</span><span class="sxs-lookup"><span data-stu-id="91c1d-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="91c1d-112">Clique na linha de uma política para ver os detalhes da política e entender por que se aplicou.</span><span class="sxs-lookup"><span data-stu-id="91c1d-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="91c1d-113">**Ferramentas para resolver problemas numa política de acesso condicional**</span><span class="sxs-lookup"><span data-stu-id="91c1d-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="91c1d-114">O modo apenas de relatório permite avaliar uma política sem afetar os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="91c1d-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="91c1d-115">E se a ferramenta permite simular eventos de inscrição e ver quais as políticas que se aplicam.</span><span class="sxs-lookup"><span data-stu-id="91c1d-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="91c1d-116">Insights e relatórios mostram o impacto em tempo real de cada política.</span><span class="sxs-lookup"><span data-stu-id="91c1d-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="91c1d-117">**Políticas de Proteção de Bases**</span><span class="sxs-lookup"><span data-stu-id="91c1d-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="91c1d-118">As políticas de proteção da linha de base foram depreciadas.</span><span class="sxs-lookup"><span data-stu-id="91c1d-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="91c1d-119">Já não estão a ser aplicadas e em breve serão removidas do portal Azure.</span><span class="sxs-lookup"><span data-stu-id="91c1d-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="91c1d-120">Recomendamos permitir [incumprimentos de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="91c1d-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="91c1d-121">Para mais informações sobre acesso condicional consulte:</span><span class="sxs-lookup"><span data-stu-id="91c1d-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="91c1d-122">[Melhores práticas para acesso condicional no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condições de Acesso](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 Condicional [Controlos no Acesso](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 Condicional [Localizações em Acesso Condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="91c1d-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
