---
title: Não é possível iniciar sessão no Teams devido ao erro autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932035"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Não é possível iniciar sessão no Teams devido ao erro autologon.microsoftazuread-sso dot com:443

Se o SSO Totalmente Integrado estiver ativado como autenticação do O365, o URL "autologon.microsoftazuread-sso.com" poderá ter de ser adicionado aos Sites da Intranet.  Se este tiver sido adicionado anteriormente aos Sites Fidedignos e se o SSO Totalmente Integrado estiver a ser utilizado, deverá ser removido dos Sites Fidedignos.

Consulte a [Lista de Verificação de Problemas com o SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Siga estes passos para adicionar um URL à lista de Sites intranet:

1. Abra o Internet Explorer ao clicar no botão **Iniciar**. Na caixa de pesquisa, escreva Internet Explorer e, em seguida, na lista de resultados, clique **Internet Explorer**.
2. Clique em **Ferramentas** e, em seguida, clique em **opções de Internet**.
3. Clique no separador **Segurança**.
4. Agora, clique em **sites da Intranet Local**, em seguida, no botão **sites** e, finalmente, no botão **Avançadas**.
5. Introduza o URL do Site e clique em **Adicionar**.
6. Quando terminar, clique em **Fechar**.

Para mais informações, consulte [Documentação para a implementação de SSO Totalmente Integrado para o O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inclui processo baseado em Políticas para adicionar um URL aos Sites Intranet no passo 3).
