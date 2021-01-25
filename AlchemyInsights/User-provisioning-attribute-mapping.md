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
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="d7562-102">Mapeamento de atributos de fornecimento do utilizador</span><span class="sxs-lookup"><span data-stu-id="d7562-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="d7562-103">Para resolver problemas conhecidos de mapeamento de atributos, consulte [os mapeamentos do Atributo](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="d7562-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="d7562-104">O Microsoft Azure Ative Directory (AD) fornece suporte para o fornecimento de utilizadores a aplicações SaaS de terceiros, tais como Salesforce, G Suite e outros.</span><span class="sxs-lookup"><span data-stu-id="d7562-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="d7562-105">Se ativar o fornecimento de um pedido saaS de terceiros, o portal Azure controla os seus valores de atributos através de mapeamentos de atributos.</span><span class="sxs-lookup"><span data-stu-id="d7562-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="d7562-106">Para saber como personalizar os mapeamentos de atributos padrão, consulte [Personalizar o fornecimento de mapeamentos de atributos para aplicações SaaS no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="d7562-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="d7562-107">Para saber mais sobre o fornecimento de utilizadores de aplicações SaaS, veja [o que é o fornecimento automatizado de utilizadores de aplicações SaaS em Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="d7562-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="d7562-108">Ao personalizar os mapeamentos de atributos para o fornecimento do utilizador, poderá descobrir que o atributo que pretende mapear não aparece na lista de atributos Source.</span><span class="sxs-lookup"><span data-stu-id="d7562-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="d7562-109">O [Sync um atributo do seu Ative Directory para Azure AD para provisionar um artigo de aplicação mostra-lhe](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) como adicionar o atributo em falta sincronizando-o do seu AD no local para Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d7562-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
