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
# <a name="authentication-app"></a>App de autenticação

Se você é um Administrador Global, você pode rapidamente descobrir o que aconteceu ou diagnosticar problemas relacionados com o utilizador-iniciar-se usando o [Diagnóstico de Iniciarções](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Inicie os diagnósticos clicando no botão "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)". 
1. Encontre o evento para analisar inserindo nos detalhes que tem sobre o utilizador, aplicação, hora de entrada, Id de pedido ou Id de correlação.
1. Reveja os resultados de diagnóstico mostrando os detalhes do que aconteceu e que ações pode tomar para fazer alterações, se forem necessárias alterações.

**Verifique o cenário aplicável:**

1. Se um utilizador não estiver a receber uma notificação push na aplicação Microsoft Authenticator, verifique se não são apresentados sob os utilizadores bloqueados da MFA, conforme descrito no [Bloco e desbloqueie os utilizadores](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Se o utilizador não estiver bloqueado para MFA mas não receber uma notificação push, pode abrir a aplicação Microsoft Authenticator, que irá retirar os pedidos de aprovação pendentes.
1. Como um método de entrada alternativa, o utilizador também pode clicar em Iniciar sção de outra forma e escolher usar um código de verificação da minha aplicação móvel.
1. A App autenticador da Microsoft é o único método disponível para muitos utilizadores. [Saiba mais sobre os padrão de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), verifique [a App FAQ do Autenticador](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) para obter perguntas comumente feitas e como resolvê-las.
 
**Vídeos Recomendados**

[Como configurar a App Autenticador num novo telefone (2 min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
