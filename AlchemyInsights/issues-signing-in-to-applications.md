---
title: Questões de inscrição nas candidaturas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901329"
---
# <a name="issues-signing-in-to-applications"></a>Questões de inscrição nas candidaturas

Para detetar a causa ou diagnosticar problemas relacionados com a inscrição do utilizador, execute os seguintes passos:

1. Lançar o [Diagnóstico de Inscrição](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Encontre o evento para analisar introduzindo os detalhes que tem sobre o utilizador, aplicação, hora de iniciar singing, Id de pedido ou Id de correlação.
3. Reveja os resultados de diagnóstico mostrando os detalhes do que aconteceu e que ações pode tomar para fazer alterações, se forem necessárias alterações.

Seguem-se algumas questões comuns que poderá experimentar ao iniciar sessão nas candidaturas:

1. Você ou o utilizador **completou um sinal de AD Azure, mas estão a ver uma solicitação inesperada** - Consulte os artigos Pedido de consentimento inesperado ao iniciar [sessão numa aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) e [erro inesperado ao efetuar o consentimento de uma aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Você ou um utilizador **inscreveu-se diretamente numa aplicação, mas não pode inscrevê-la a partir de um deeplink no portal personalizado ou no painel de acesso**: Veja [problemas de resolução de problemas a iniciar sessão numa aplicação a partir de Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Você ou um utilizador **completou um sinal AD Azure, mas a aplicação apresenta uma mensagem de erro e não deixa o utilizador terminar o fluxo de entrada** de entrada : O problema é que a aplicação não aceitou a resposta que o Azure AD emitiu. Siga [estes passos](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) para resolver problemas.
4. Você ou um utilizador **não pode iniciar sessão numa aplicação não-galeria configurada para o sign-on de senha única**: Siga as orientações [nestes passos](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) para resolver problemas.
5. Você ou um utilizador **não pode iniciar sessão numa aplicação da Galeria AD Azure configurada para uma única sessão de assinatura**: Siga estes [passos](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) para resolver problemas.
6. Você ou um utilizador **não podem iniciar sessão numa aplicação da Microsoft**: Siga estes [passos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) para resolver problemas.
7. Você ou um utilizador **não pode inscrever-se numa aplicação não-galeria configurada para um único sinal federado**: Siga [estes passos](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) para resolver problemas.
8. Você ou um utilizador **não pode inscrever-se numa aplicação da Galeria AD Azure configurada para um único sinal federado**: Siga [estes passos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para resolver problemas.
9. Você ou um utilizador **não podem iniciar sessão numa aplicação desenvolvida sob medida**: Siga estes [passos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para resolver problemas.
10. Você ou um utilizador **não pode iniciar sessão numa aplicação no local utilizando o proxy da aplicação AZure AD**: Siga [estes passos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) para resolver problemas.

