---
title: Configurar e prolongar as vidas simbólicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917008"
---
# <a name="configure-and-extend-token-lifetimes"></a>Configurar e prolongar as vidas simbólicas

Pode especificar o tempo de vida útil de um token de acesso, SAML ou ID emitido pela plataforma de identidade Microsoft. Você pode definir vidas simbólicas para todas as aplicações da sua organização, para uma aplicação multi-inquilina (multi-organização) ou para um diretor de serviço específico na sua organização. Para mais informações, leia [as vidas simbólicas configuráveis.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

Por exemplo, leia [exemplos de como configurar vidas simbólicas.](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)

Para aprender a configurar a vida e a compatibilidade de um símbolo em Azure Ative Directory B2C (Azure AD B2C), consulte [fichas de configuração no Azure Ative Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

O artigo [Configurar o comportamento da sessão no Azure Ative Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descreve os métodos de assinatura única (SSO) utilizados no Azure AD B2C e ajuda-o a escolher o método SSO mais adequado ao configurar a sua política.

**Quanto tempo duram as fichas? Por quanto tempo são válidos?**

As vidas simbólicas são de 1 hora e a vida útil da sessão é de 24 horas. Isto significa que, se não houver pedidos em 24 horas, terá de fazer login novamente antes de pedir um novo token.

> [!NOTE]
> Depois de 30 de maio de 2020, nenhum novo inquilino poderá usar a política de Vida Token Configurada para configurar sessão e refrescar tokens. A depreciação acontecerá dentro de alguns meses, o que significa que deixaremos de honrar a sessão existente e refrescaremos as polícias. Ainda pode configurar o acesso a vidas simbólicas após a depreciação.






