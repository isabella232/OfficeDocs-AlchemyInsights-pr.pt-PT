---
title: Problemas de inscrição do utilizador SSO sem emenda
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935178"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problemas de inscrição do utilizador SSO sem emenda

Após a autenticação do utilizador, o navegador irá cache nas credenciais do utilizador, de modo que no mesmo navegador, a aplicação irá automaticamente iniciar scontabilidade com a mesma conta. Isto pode dificultar que outro utilizador ou um único utilizador faça login em várias contas num dispositivo. Para resolver isto: 1. Tente iniciar sessão noutro navegador. 2. Limpe o cache do navegador e/ou cookies e tente iniciar sessão novamente.

Se ainda estiver a ter problemas de inscrição, recomendamos que diagnostice e automatize as etapas de resolução:

1. Instale a [Extensão de Navegador My Apps Secure](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) para ajudar o Azure Ative Directory (Azure AD) a fornecer um melhor diagnóstico e resoluções ao utilizar a experiência de teste no portal Azure.
2. Reproduza o erro utilizando a experiência de teste na página de configuração da aplicação no portal Azure. Para saber mais, consulte [as aplicações de inscrição única baseadas em Debug SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Se utilizar a experiência de teste no portal Azure com a extensão do navegador My Apps Secure, pode saltar o **passo 4**.
4. Para abrir a página de configuração única baseada em SAML:
    - Abra o [portal Azure](https://portal.azure.com/) e inscreva-se como **Administrador Global** ou **Coadmin**.
    - Abra a **Extensão do Diretório Ativo Azure** selecionando **todos os serviços** no topo do menu principal de navegação do lado esquerdo.
    - Digite "Azure Ative Directory" na caixa de pesquisa do filtro e selecione o item **Azure Ative Directory.**
    - Selecione **Aplicações empresariais** do menu de navegação à esquerda do Azure Ative.
    - Selecione **Todas as Aplicações** para ver uma lista de todas as suas aplicações. Se não vir a aplicação deseja aparecer aqui, utilize o controlo **filter** no topo da Lista de **Todas as Aplicações** e desate a opção **'Mostrar'** para **todas as aplicações**.
    - Selecione a aplicação que pretende configurar para uma única sação.
    - Depois das cargas de aplicação, selecione **'Único's sign-on'** no menu de navegação à esquerda da aplicação.
    - Selecione **SSO baseado em SAML.**
5. Com base no erro, para saber mais sobre os passos recomendados a seguir, consulte [problemas de sessão em aplicações configuradas com base em SEM.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Para resolver outros problemas de sinalização do utilizador, consulte as seguintes orientações:
    - [Protocolo SAML de Sign-On único](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Como: Erros de sessão de resolução de problemas utilizando relatórios do Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Pedido de consentimento inesperado](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Erro de consentimento do utilizador](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemas de sessão a partir de My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Erro na página de inscrição da aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problema de assinatura de uma App da Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
