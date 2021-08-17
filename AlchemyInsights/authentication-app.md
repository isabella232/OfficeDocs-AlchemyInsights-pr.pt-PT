---
title: Aplicação de autenticação
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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082953"
---
# <a name="authentication-app"></a>Aplicação de autenticação

Se for um Administrador Global, pode descobrir rapidamente o que aconteceu ou diagnosticar problemas relacionados com o iniciar a sua conta ao utilizar os Diagnósticos de Iniciar [a Sua Conta.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Inicie o diagnóstico ao clicar[no botão](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" Iniciar Diagnóstico ". 
1. Encontre o evento para analisar ao introduzir os detalhes que tem sobre o utilizador, aplicação, hora de entrada, ID do Pedido ou ID de correlação.
1. Reveja os resultados de diagnóstico que mostram os detalhes do que aconteceu e que ações pode tomar para fazer alterações, se for necessário fazer alterações.

**Verifique o cenário aplicável:**

1. Se um utilizador não estiver a receber uma notificação push na aplicação Microsoft Authenticator, verifique se não são apresentados na aplicação MFA bloqueada, conforme descrito em Bloquear e desbloquear [utilizadores.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Se o utilizador não estiver bloqueado para a autarca mas não receber uma notificação push, pode abrir a aplicação Microsoft Authenticator, o que irá pedir os pedidos de aprovação pendentes.
1. Como método de acesso alternativo, o utilizador também pode clicar em Assinar de outra forma e escolher utilizar um código de verificação a partir da minha aplicação para dispositivos móveis.
1. A Microsoft Authenticator App é o único método disponível para muitos utilizadores. [Saiba mais sobre as predefinições](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)de segurança , [consulte Authenticator FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) da Aplicação para perguntas mais frequentes e sobre como resolvê-las.
 
**Vídeos Recomendados**

[Como configurar a Authenticator Aplicação num novo telemóvel (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
