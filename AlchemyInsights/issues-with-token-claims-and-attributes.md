---
title: Problemas com Atributos e Afirmações de Token
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012895"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemas com Atributos e Afirmações de Token

**Atualizar, configurar ou remover reivindicações de tokens**

1. Ao utilizar Azure Active Directory (Azure AD), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) pode personalizar o tipo de reclamação para a reclamação de função no token de resposta que recebe após autorizar uma aplicação.
2. Os programadores de aplicações podem utilizar afirmações opcionais nas suas aplicações do Azure AD para especificar as afirmações que pretendem nos tokens enviados para a respetivo aplicação. Para obter mais informações, consulte [Fornecer reivindicações opcionais à sua aplicação.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configure as reclamações de grupos para aplicações com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Se estiver a utilizar o Sinal de Utilização Única Sem Complicações na sua aplicação, consulte Personalizar as reclamações emitidas no [token do SAML para aplicações empresariais.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mapeamento de Atributos da Claims**

1. Para configurar a política de mapeamento de reivindicações através do PowerShell, consulte o artigo Personalizar reclamações emitentes em tokens para uma aplicação específica num inquilino [(Pré-visualização).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Os atributos da extensão de esquema de diretório fornecem uma forma de armazenar dados adicionais no Azure Active Directory em objetos de utilizador e outros objetos de diretório, como grupos, detalhes de inquilino e principais de serviço. Apenas os atributos de extensão em objetos de utilizador podem ser utilizados para emissar reclamações de aplicações. [Utilizar atributos](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) da extensão de esquema de diretório nas afirmações descreve como utilizar atributos da extensão de esquema de diretório para enviar dados de utilizador para aplicações em afirmações de tokens.

Para obter mais informações sobre as reclamações de tokens, consulte:

- [Reclamações em tokens de acesso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Reclamações numa id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Afirmações](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que pode esperar em tokens ID e tokens de acesso emitidos pelo Azure AD B2C
- [Referência de afirmações de tokens SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
