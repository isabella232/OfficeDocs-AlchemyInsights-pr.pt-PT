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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974990"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="53823-102">Permissões e consentimento da API</span><span class="sxs-lookup"><span data-stu-id="53823-102">API permissions and consent</span></span>

<span data-ttu-id="53823-103">As aplicações que se integram com a plataforma de identidade da Microsoft seguem um modelo de autorização que dá aos utilizadores e administradores o controlo sobre a forma como os dados podem ser acedidos.</span><span class="sxs-lookup"><span data-stu-id="53823-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="53823-104">A implementação do modelo de autorização foi atualizada no ponto final da plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="53823-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="53823-105">Altera a forma como uma aplicação deve interagir com a plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="53823-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="53823-106">[Permissões e consentimento no ponto final da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) abrange os conceitos básicos deste modelo de autorização, incluindo âmbitos, permissões e consentimento.</span><span class="sxs-lookup"><span data-stu-id="53823-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="53823-107">O [quadro de consentimento do Azure Ative Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita o desenvolvimento de aplicações de clientes multi-inquilinos e clientes nativos.</span><span class="sxs-lookup"><span data-stu-id="53823-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="53823-108">Estas aplicações permitem a inscrição por conta de utilizador de um inquilino AZure AD que é diferente daquele em que a aplicação está registada.</span><span class="sxs-lookup"><span data-stu-id="53823-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="53823-109">Podem também ter de aceder a APIs web, como a API do Microsoft Graph (para aceder a Azure AD, Intune e serviços na Microsoft 365) e a APIs de outros serviços da Microsoft, além das suas próprias APIs web.</span><span class="sxs-lookup"><span data-stu-id="53823-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

