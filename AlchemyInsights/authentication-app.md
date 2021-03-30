---
title: App de autenticação
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405677"
---
# <a name="authentication-app"></a><span data-ttu-id="fcb67-102">App de autenticação</span><span class="sxs-lookup"><span data-stu-id="fcb67-102">Authentication app</span></span>

<span data-ttu-id="fcb67-103">Se você é um Administrador Global, você pode rapidamente descobrir o que aconteceu ou diagnosticar problemas relacionados com o utilizador-iniciar-se usando o [Diagnóstico de Iniciarções](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="fcb67-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="fcb67-104">Inicie os diagnósticos clicando no botão "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)".</span><span class="sxs-lookup"><span data-stu-id="fcb67-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="fcb67-105">Encontre o evento para analisar inserindo nos detalhes que tem sobre o utilizador, aplicação, hora de entrada, Id de pedido ou Id de correlação.</span><span class="sxs-lookup"><span data-stu-id="fcb67-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="fcb67-106">Reveja os resultados de diagnóstico mostrando os detalhes do que aconteceu e que ações pode tomar para fazer alterações, se forem necessárias alterações.</span><span class="sxs-lookup"><span data-stu-id="fcb67-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="fcb67-107">**Verifique o cenário aplicável:**</span><span class="sxs-lookup"><span data-stu-id="fcb67-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="fcb67-108">Se um utilizador não estiver a receber uma notificação push na aplicação Microsoft Authenticator, verifique se não são apresentados sob os utilizadores bloqueados da MFA, conforme descrito no [Bloco e desbloqueie os utilizadores](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="fcb67-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="fcb67-109">Se o utilizador não estiver bloqueado para MFA mas não receber uma notificação push, pode abrir a aplicação Microsoft Authenticator, que irá retirar os pedidos de aprovação pendentes.</span><span class="sxs-lookup"><span data-stu-id="fcb67-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="fcb67-110">Como um método de entrada alternativa, o utilizador também pode clicar em Iniciar sção de outra forma e escolher usar um código de verificação da minha aplicação móvel.</span><span class="sxs-lookup"><span data-stu-id="fcb67-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="fcb67-111">A App autenticador da Microsoft é o único método disponível para muitos utilizadores.</span><span class="sxs-lookup"><span data-stu-id="fcb67-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="fcb67-112">[Saiba mais sobre os padrão de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), verifique [a App FAQ do Autenticador](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) para obter perguntas comumente feitas e como resolvê-las.</span><span class="sxs-lookup"><span data-stu-id="fcb67-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="fcb67-113">**Vídeos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="fcb67-113">**Recommended Videos**</span></span>

<span data-ttu-id="fcb67-114">[Como configurar a App Autenticador num novo telefone (2 min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fcb67-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
