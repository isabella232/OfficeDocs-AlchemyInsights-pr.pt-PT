---
title: Segredo do cliente Registo de Aplicações ou Problemas com o Certificado
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951504"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Segredo do cliente Registo de Aplicações ou Problemas com o Certificado

O segredo do cliente da aplicação está a expirar?

Independentemente da forma como a aplicação registada foi criada, quer através do processo de registo padrão no portal Registo de Aplicações ou se o Principal de Serviço foi criado no seu inquilino através do consentimento da aplicação, tem de ser criado um novo Segredo de Cliente antes da expiração do atual e atualizado no código de aplicação relacionado. O período de validade máximo é de 2 anos. Como lembrete, o valor secreto tem de ser registado, uma vez que deixará de estar visível depois de sair da página Registos de aplicações no portal. Para obter mais informações, consulte [Guia de Utilização:](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) Registar uma aplicação no plataforma de identidades da Microsoft e [Práticas recomendadas para a plataforma de identidades da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Para saber mais, consulte [Criar uma aplicação do Azure AD & principal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)de serviço no portal – plataforma de identidades da Microsoft .
