---
title: Configurar o sign-on único sem emenda (SSO)
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841676"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurar o sign-on único sem emenda (SSO)

**Configure aplicações**

1. Deve obter os valores do vendedor de aplicações. Pode introduzir manualmente os valores ou carregar um ficheiro de metadados para extrair o valor dos campos.
2. Muitas aplicações já foram pré-configuradas para trabalhar com a Azure AD. Estas aplicações estão listadas na galeria de aplicações que pode navegar quando adiciona uma aplicação ao seu inquilino AZure AD. A [série quickstart](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) acompanha-o através do processo.
3. Para criar uma aplicação não-galeria, pode clicar em + Criar o seu próprio botão **De aplicação** e dar um nome à sua Aplicação.
    - Por predefinição, irá **selecionar Integrar qualquer outra aplicação que não encontre na galeria,** que é a opção correta para aplicações não-galeria.
    - Assim que atingir **a Create** depois de colocar o nome para a aplicação, criará uma nova Aplicação Empresarial não-galeria.
    - Em seguida, poderá navegar para **o Single Sign-on em** **Gestão** dessa aplicação e poderá ver diferentes técnicas para implementá-la no seu ambiente.

**Configure sSO sem emenda para uma aplicação específica**

Para as aplicações na galeria encontrará instruções detalhadas, passo a passo. Para aceder aos passos pode navegar numa lista de todos os tutoriais de configuração de aplicações nos [tutoriais de configuração de aplicações SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Configurar SSO baseado em SAML**

1. [Quickstart: Configurar um único sign-on (SSO) baseado em SAML para uma aplicação no seu inquilino Azure Ative Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Para saber mais sobre a opção baseada em SAML para um único sign-on, consulte [Understand SAML single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Para saber mais sobre os pedidos e respostas de autenticação SAML 2.0 que o Azure Ative Directory (Azure AD) suporta para Sign-On Individuais (SSO), consulte [o protocolo SAML de Sign-On Único](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Para aprender a criar e configurar um sign-on único baseado em SAML (SSO) para a sua aplicação no Azure Ative Directory (AD) utilizando a API do Gráfico da Microsoft, consulte um [único sinal baseado em SAML para a sua aplicação utilizando a API do Gráfico microsoft](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Para saber como a Azure AD utiliza o protocolo SAML, consulte [como a plataforma de identidade da Microsoft utiliza o protocolo SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Configure tokens e reclamações**

1. [Como: personalizar reclamações emitidas no token SAML para aplicações empresariais](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Para aprender a configurar reclamações usando o PowerShell, consulte [Como: Personalizar reclamações emitidas em fichas para uma aplicação específica num inquilino (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Para aprender a configurar reclamações opcionais, consulte [Como: Fornecer reclamações opcionais à sua aplicação.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Para aprender a utilizar atributos de extensão de esquema de diretório para enviar dados do utilizador a aplicações em alegações simbólicas, consulte [utilizar atributos de extensão de esquema de diretório em sinistros](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Para aprender a configurar vidas simbólicas, consulte [as vidas de símbolos configurantes na plataforma de identidade da Microsoft (pré-visualização)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Configure políticas de vida simbólicas (pré-visualização)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Neste artigo, passamos por um cenário político comum que pode ajudá-lo a impor novas regras para a vida útil simbólica. No exemplo, aprende-se a criar uma política que exige que os utilizadores autentem mais frequentemente na sua aplicação web.

**Configuração SSO resolução de problemas**

- Para perguntas frequentes sobre O Diretório Ativo sem emenda sem emenda Sign-On (Seamless SSO), consulte [O Diretório Ativo Sem Emenda Sem Emenda Sign-On: Perguntas frequentes.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Para obter informações sobre problemas comuns relativos ao Azure Ative Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), consulte O Sinal Único Sem Emenda sem emenda do Diretório Sem Emenda da [Resolução de Problemas](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
