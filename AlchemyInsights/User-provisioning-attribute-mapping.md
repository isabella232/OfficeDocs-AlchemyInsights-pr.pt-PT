---
title: Mapeamento de atributos de fornecimento do utilizador
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949892"
---
# <a name="user-provisioning-attribute-mapping"></a>Mapeamento de atributos de fornecimento do utilizador

1. Para resolver problemas conhecidos de mapeamento de atributos, consulte [os mapeamentos do Atributo](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. O Microsoft Azure Ative Directory (AD) fornece suporte para o fornecimento de utilizadores a aplicações SaaS de terceiros, tais como Salesforce, G Suite e outros. Se ativar o fornecimento de um pedido saaS de terceiros, o portal Azure controla os seus valores de atributos através de mapeamentos de atributos. Para saber como personalizar os mapeamentos de atributos padrão, consulte [Personalizar o fornecimento de mapeamentos de atributos para aplicações SaaS no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Para saber mais sobre o fornecimento de utilizadores de aplicações SaaS, veja [o que é o fornecimento automatizado de utilizadores de aplicações SaaS em Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Ao personalizar os mapeamentos de atributos para o fornecimento do utilizador, poderá descobrir que o atributo que pretende mapear não aparece na lista de atributos Source. O [Sync um atributo do seu Ative Directory para Azure AD para provisionar um artigo de aplicação mostra-lhe](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) como adicionar o atributo em falta sincronizando-o do seu AD no local para Azure AD.
