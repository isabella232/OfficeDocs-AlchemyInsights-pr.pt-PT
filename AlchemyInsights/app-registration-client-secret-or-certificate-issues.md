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
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="13b96-102">Problemas secretos ou certificados do cliente do Registo de Aplicações</span><span class="sxs-lookup"><span data-stu-id="13b96-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="13b96-103">O segredo do cliente da aplicação expira?</span><span class="sxs-lookup"><span data-stu-id="13b96-103">Application client secret expiring?</span></span>

<span data-ttu-id="13b96-104">Independentemente da forma como a aplicação registada foi criada, seja através do processo de registo padrão no portal de Registo de Aplicações ou se o Diretor de Serviço foi criado no seu arrendatário através do consentimento da candidatura, terá de ser criado um novo Cliente Segredo antes da expiração do atual e atualizado no código de aplicação relacionado.</span><span class="sxs-lookup"><span data-stu-id="13b96-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="13b96-105">O prazo máximo de validade é de 2 anos.</span><span class="sxs-lookup"><span data-stu-id="13b96-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="13b96-106">Como lembrete, o valor secreto deve ser registado, uma vez que deixará de ser visível depois de sair da página de registos da App no portal.</span><span class="sxs-lookup"><span data-stu-id="13b96-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="13b96-107">Para obter mais informações, consulte [Quickstart: Registe uma aplicação na plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) e as [melhores práticas para a plataforma de identidade da Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="13b96-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="13b96-108">Para saber mais, consulte [Criar uma aplicação AD AD & principal no portal - plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="13b96-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
