---
title: Problemas secretos ou certificados do cliente do Registo de Aplicações
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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405336"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemas secretos ou certificados do cliente do Registo de Aplicações

O segredo do cliente da aplicação expira?

Independentemente da forma como a aplicação registada foi criada, seja através do processo de registo padrão no portal de Registo de Aplicações ou se o Diretor de Serviço foi criado no seu arrendatário através do consentimento da candidatura, terá de ser criado um novo Cliente Segredo antes da expiração do atual e atualizado no código de aplicação relacionado. O prazo máximo de validade é de 2 anos. Como lembrete, o valor secreto deve ser registado, uma vez que deixará de ser visível depois de sair da página de registos da App no portal. Para obter mais informações, consulte [Quickstart: Registe uma aplicação na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) e as [melhores práticas para a plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Para saber mais, consulte [Criar uma aplicação AD AD & principal no portal - plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
