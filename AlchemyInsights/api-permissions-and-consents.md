---
title: Permissões e Consentimento da API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932108"
---
# <a name="api-permissions-and-consent"></a>Permissões e consentimento da API

As aplicações integradas com plataforma de identidades da Microsoft seguem um modelo de autorização que permite aos utilizadores e administradores controlar a forma como os dados podem ser acetidos. A implementação do modelo de autorização foi atualizada no ponto plataforma de identidades da Microsoft final. Altera a forma como uma aplicação tem de interagir com a plataforma de identidades da Microsoft. [As permissões e a](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) autorização no plataforma de identidades da Microsoft abrangem os conceitos básicos deste modelo de autorização, incluindo âmbitos, permissões e consentimento.

A Azure Active Directory estrutura de consentimento [do Azure Active Directory Azure AD](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) torna mais fácil desenvolver aplicações cliente multi-inquilino e nativas. Estas aplicações permitem o registo de contas de utilizador por parte de um inquilino do Azure AD diferente daquele em que a aplicação está registada. Também poderão ter de aceder às APIs Web, como a API do Microsoft Graph (para aceder ao Azure AD, Intune e serviços no Microsoft 365) e a outras APIs do serviços Microsoft, além das suas próprias APIs Web.

