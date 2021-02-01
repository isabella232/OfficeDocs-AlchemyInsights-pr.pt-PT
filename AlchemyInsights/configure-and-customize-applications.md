---
title: Configurar e personalizar aplicações
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063662"
---
# <a name="configure-and-customize-applications"></a>Configurar e personalizar aplicações

**Configure aplicações**

1. [Quickstart: Configure propriedades para uma aplicação no seu inquilino Azure Ative Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) mostra-lhe como configurar algumas das propriedades para uma aplicação.
2. Para ajudar a integrar as suas aplicações com o Azure Ative Directory, desenvolvemos [uma coleção de tutoriais](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) que o acompanham através da configuração.
3. [Como configurar uma aplicação Proxy de aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) ajuda-o a entender como configurar uma aplicação Proxy de aplicação dentro da Azure AD para expor as suas aplicações no local à nuvem.
4. [Baixar PingAccess e configurar a sua aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): Siga as instruções em *Configure PingAccess para Azure AD para proteger aplicações publicadas* usando o Microsoft Azure AD Application Proxy no site ping Identity e descarregue a versão mais recente do PingAccess.

**Erros de aplicação mal configurados (AADSTS650056)**

1. Certifique-se de que está a aceder à aplicação a partir do endereço de inscrição fornecido pelo proprietário da aplicação. Caso contrário, significar, inscreva-se na aplicação através do seu processo normal. Na maioria dos casos, isto irá resolver-se automaticamente naturalmente. Se não, então este post pode ajudar a resolver problemas e resolvê-lo.
2. **Se a sua organização possuir a aplicação** (o que significa que o registo de candidatura está na sua organização):
    - No mínimo, recomendamos que seja adicionada a `User.Read` permissão ou `openid` delegada do **Microsoft Graph.**
    - Certifique-se de que o pedido e todas as suas permissões são consentidas. Pode verificar isto olhando para a coluna **de Estado** do registo do Pedido no âmbito das **Permissões API.**
    - Em alguns cenários, a aplicação pode ser de terceiros, no entanto pode ser registada na sua organização. Confirme se esta aplicação está listada nos registos da sua App (Não aplicações Da Empresa).
    - Se continuar a ver esta mensagem de erro. Em seguida, poderá ser necessário construir o URL de consentimento descrito no **passo 4**.
3. **Se a sua organização não for a proprietária da aplicação e a sua utilização como aplicação de terceiros:**
    - Se for o administrador da Global/Empresa, deverá ver o ecrã de consentimento. Certifique-se de verificar a caixa para **"Consent em nome da sua organização".**
    - Se não vir o ecrã de consentimento, elimine a aplicação Enterprise e tente novamente.
    - Se continuar a ver esta mensagem de erro. Em seguida, poderá ser necessário construir o URL de consentimento descrito no **passo 4**.
4. **Construa manualmente o URL de consentimento a ser utilizado**: Se a aplicação for concebida para aceder a um recurso específico, poderá não ser capaz de utilizar os botões Consentimento a partir do portal Azure, terá de gerar manualmente o seu próprio URL de consentimento e usá-lo.
    - Terá de obter `{App-Id}` o e o `{App-Uri-Id}` do proprietário da aplicação. `{Tenant-Id}` será o seu identificador de inquilino. Isto será `yourdomain.onmicrosoft.com` ou a sua identificação de diretório.
    - Se a aplicação estiver a aceder-se ao recurso, então o `{App-Id}` e será o `{App-Uri-Id}` mesmo.
5. Para obter mais informações, consulte [problemas de sessão de inscrição em aplicações configuradas com base em SEML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizar Aplicações**

- [Adicione marca à página de inscrição do Azure Ative Directory da sua organização](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) - Use o logótipo da sua organização e esquemas de cores personalizados para fornecer um look-and-feel consistente às suas páginas de inscrição do Azure Ative Directory (Azure AD).
- [Adicione o seu nome de domínio personalizado utilizando o portal Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - Cada novo inquilino AZure AD vem com um nome de domínio inicial. Não é possível alterar ou apagar o nome de domínio inicial, mas pode adicionar os nomes da sua organização. Adicionar nomes de domínio personalizados ajuda a criar nomes de utilizadores que sejam familiares aos seus utilizadores.
