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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044999"
---
# <a name="configure-and-customize-applications"></a>Configurar e personalizar aplicações

**Configurar Aplicações**

1. Guia de Instrução: configurar propriedades para uma aplicação no seu inquilino [do Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) mostra-lhe como configurar algumas das propriedades de uma aplicação.
2. Para ajudar a integrar as suas aplicações com Azure Active Directory, desenvolvemos uma coleção de [tutoriais](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) que o guiam pela configuração.
3. Como configurar uma aplicação [Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) de Aplicação ajuda-o a compreender como configurar uma aplicação Proxy de Aplicação no Azure AD para expor as suas aplicações no local à nuvem.
4. Transfira o [PingAccess e configure](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)a sua aplicação: siga as instruções em Configurar *O PingAccess para o Azure AD* para proteger as aplicações publicadas com o Microsoft Azure AD Application Proxy no site da Identidade do Ping e transfira a versão mais recente do PingAccess.

**Erros de Aplicação Mal Configurada (AADSTS650056)**

1. Certifique-se de que está a aceder à aplicação a partir do endereço de inscrição fornecido pelo proprietário da aplicação. Caso contrário, inscreva-se na aplicação através do seu processo normal. Na maioria dos casos, esta solução será resolvida automaticamente de forma natural. Se tal não acontecer, esta publicação poderá ajudar a resolver o problema.
2. **Se a sua organização for a deteta a aplicação** (ou seja, se o registo da aplicação estiver na sua organização):
    - No mínimo, recomendamos a permissão `User.Read` `openid` delegada ou do **Microsoft Graph** ser adicionada.
    - Certifique-se de que a aplicação e todas as suas permissões estão consentidos. Pode verificar esta situação ao ver a coluna Estado **do** Registo de aplicações nas Permissões **da API.**
    - Em alguns cenários, a aplicação poderá ser de terceiros, no entanto, poderá estar registada na sua organização. Confirme se esta aplicação está listada nos registos da Aplicação (Não nas aplicações Enterprise).
    - Se continuar a ver esta mensagem de erro. Poderá ter de criar o URL de consentimento descrito **no passo 4.**
3. **Se a sua organização não for o proprietário da aplicação e a utilizar como uma aplicação de terceiros:**
    - Se for o administrador Global/Company, deverá ver o ecrã de consentimento. Certifique-se de que verifica a **caixa "Consentimento em nome da sua organização".**
    - Se não vir o ecrã de consentimento, elimine a aplicação Enterprise e tente novamente.
    - Se continuar a ver esta mensagem de erro. Poderá ter de criar o URL de consentimento descrito **no passo 4.**
4. Criar manualmente o **URL** de consentimento para ser utilizado: Se a aplicação tiver sido concebida para aceder a um recurso específico, poderá não conseguir utilizar os botões de Consentimento a partir do portal do Azure, terá de gerar manualmente o seu próprio URL de consentimento e utilizar este.
    - Terá de obter o e `{App-Id}` o do proprietário da `{App-Uri-Id}` aplicação. `{Tenant-Id}` será o seu identificador de inquilino. Será o seu `yourdomain.onmicrosoft.com` ID de diretório.
    - Se a aplicação estiver a aceder a si própria para o recurso, `{App-Id}` o e será o `{App-Uri-Id}` mesmo.
5. Para obter mais informações, consulte Problemas ao entrar em aplicações configuradas configuradas com base em [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizar Aplicações**

- Adicionar imagem [branding](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) à página de início de sessão do Azure Active Directory da sua organização - Utilize o logótipo da sua organização e esquemas de cores personalizados para fornecer um asste e uma imagem consistentes às páginas de início de sessão do Azure Active Directory (Azure AD).
- [Adicione o seu nome de domínio personalizado](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) utilizando o portal Azure Active Directory – todos os novos inquilinos do Azure AD vêm com um nome de domínio inicial. Não pode alterar ou eliminar o nome de domínio inicial, mas pode adicionar os nomes da sua organização. Adicionar nomes de domínio personalizados ajuda-o a criar nomes de utilizador que sejam familiares para os seus utilizadores.
