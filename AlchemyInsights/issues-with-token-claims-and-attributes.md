---
title: Problemas com reclamações e atributos token
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035969"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemas com reclamações e atributos token

**Atualizar, configurar ou remover reclamações simbólicas**

1. Ao utilizar o Azure Ative Directory (Azure AD), pode [personalizar o tipo de reclamação para a reivindicação de funções](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) no token de resposta que recebe depois de autorizar uma aplicação.
2. Os desenvolvedores de aplicações podem usar reclamações opcionais nas suas aplicações AZure AD para especificar quais as alegações que pretendem em fichas enviadas para a sua aplicação. Para obter mais informações, consulte [Fornecer reclamações opcionais à sua aplicação.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configure pedidos de pedidos de candidaturas com a Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Se utilizar o 'Sign-on' único sem emenda na sua aplicação, consulte [as reclamações personalizadas emitidas no token SAML para aplicações empresariais](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Mapeamento de atributos de reclamações**

1. Para configurar a política de mapeamento de reclamações utilizando o PowerShell, consulte [Personalizar reclamações emitidas em fichas para uma aplicação específica num inquilino (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Os atributos de extensão de esquema de diretório fornecem uma forma de armazenar dados adicionais no Azure Ative Directory em objetos de utilizador e outros objetos de diretório, tais como grupos, detalhes do inquilino, diretores de serviço. Apenas os atributos de extensão em objetos do utilizador podem ser usados para emitir reclamações para aplicações. [A utilização de atributos de extensão de esquema de diretório em sinistros](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) descreve como utilizar atributos de extensão de esquema de diretório para enviar dados do utilizador para aplicações em alegações simbólicas.

Para obter mais informações sobre sinistros simbólicos, consulte:

- [Reclamações em fichas de acesso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Reclamações num id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Reclamações](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que pode esperar em fichas de ID e fichas de acesso emitidas pela Azure AD B2C
- [Referência de reclamações de ficha SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
