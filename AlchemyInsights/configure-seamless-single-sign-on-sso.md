---
title: Configurar o Sinal de Ações Simples Sem Comâneo (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966048"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurar o Sinal de Ações Simples Sem Comâneo (SSO)

**Configurar Aplicações**

1. Deverá obter os valores a partir do fornecedor da aplicação. Pode introduzir os valores manualmente ou carregar um ficheiro de metadados para extrair o valor dos campos.
2. Muitas aplicações já foram pré-configuradas para funcionarem com o Azure AD. Estas aplicações estão listadas na galeria de aplicações que pode procurar quando adiciona uma aplicação ao seu inquilino do Azure AD. A [série de guias de guia](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guia-o pelo processo.
3. Para criar uma aplicação que não seja de galeria, pode clicar em **+ Criar** o seu próprio botão de Aplicação e dar um nome à sua Aplicação.
    - Por predefinição, a aplicação Irá selecionar Integrar qualquer outra aplicação que não encontrar na galeria, que é a opção correta para Aplicações que não são da galeria. 
    - Depois de chegar **a Criar** depois de colocar o nome da aplicação, será criado uma nova Aplicação Empresarial Sem Galeria.
    - Em seguida, poderá navegar  para o  Registo Único em Gerir essa aplicação e poderá ver diferentes técnicas para a implementar no seu ambiente.

**Configurar o SSO Sem Complicações para uma aplicação específica**

Para as aplicações na galeria, encontrará instruções detalhadas e passo a passo. Para aceder aos passos, pode procurar uma lista de todos os tutoriais de configuração de aplicações nos tutoriais de configuração de aplicações [SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Configurar SSO baseado em SAML**

1. Guia de Utilização Rápida: configurar o registo único (SSO) baseado em SAML para uma aplicação no seu inquilino [do Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Para saber mais sobre a opção baseada em SAML para o primeiro sinal, consulte Compreender o sinal de assinatura único baseado [em SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Para saber mais sobre os pedidos de autenticação SAML 2.0 e respostas que o Azure Active Directory (Azure AD) suporta para o Sign-On Único (SSO), consulte Protocolo [SAML Sign-On.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Para saber como criar e configurar um SSO (single sign-on) baseado em SAML para a sua aplicação no Azure Active Directory (Azure AD) através da API do Microsoft Graph, consulte Configurar o registo único baseado em SAML para a sua aplicação através da API do [Microsoft Graph.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Para saber como o Azure AD utiliza o protocolo SAML, consulte Como o [plataforma de identidades da Microsoft utiliza o protocolo SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Configurar Tokens e Reivindicações**

1. [Como: personalizar as reclamações emitidas no token SAML para aplicações empresariais.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Para saber como configurar afirmações com o PowerShell, consulte Como: Personalizar as reclamações emitidas em tokens para uma aplicação específica num inquilino [(Pré-visualização).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Para saber como configurar reivindicações opcionais, consulte Como: Fornecer [reivindicações opcionais à sua aplicação.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Para saber como utilizar atributos da extensão de esquema de diretório para enviar dados de utilizador para aplicações em afirmações de tokens, consulte Utilizar atributos da extensão de esquema de diretório nas [afirmações](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Para saber como configurar permissões de tokens, consulte o artigo Duração de [token configurável no plataforma de identidades da Microsoft (pré-visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. Configurar políticas de duração de [tokens (pré-visualização)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Neste artigo, iremos debater um cenário de política comum que pode ajudá-lo a impor novas regras para a duração dos tokens. No exemplo, vai aprender a criar uma política que exija que os utilizadores autentiquem mais frequentemente na sua aplicação Web.

**Remoção de Configuração do SSO**

- Para as perguntas mais frequentes sobre Azure Active Directory Simples totalmente Sign-On (SSO Totalmente Simples), consulte Azure Active Directory Desintroduzição Única Totalmente Simples: perguntas mais [frequentes](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Para obter informações sobre problemas comuns relacionados com o Azure Active Directory (Azure AD) Single Sign-On (SSO Sem Com problemas), consulte Resolver problemas Azure Active Directory o Sinal de Utilização Única Sem Com [problemas.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
