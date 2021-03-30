---
title: Problemas do Proprietário do Registo de Aplicações
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
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405317"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="69f37-102">Problemas do Proprietário do Registo de Aplicações</span><span class="sxs-lookup"><span data-stu-id="69f37-102">App Registration Owner issues</span></span>

<span data-ttu-id="69f37-103">Seguem-se os métodos disponíveis para adicionar os principais como proprietários para registos de aplicações:</span><span class="sxs-lookup"><span data-stu-id="69f37-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="69f37-104">Usando módulo Ad PowerShell -</span><span class="sxs-lookup"><span data-stu-id="69f37-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="69f37-105">Referência: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="69f37-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="69f37-106">Usando O Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="69f37-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="69f37-107">Referência: [az ad app proprietário](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="69f37-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="69f37-108">Usando o Ms Graph -</span><span class="sxs-lookup"><span data-stu-id="69f37-108">Using MS Graph -</span></span>

    <span data-ttu-id="69f37-109">Referência: [Adicionar proprietário - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="69f37-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="69f37-110">Utilização do Portal AD Azure - Navegue para [portal.azure.com](https://portal.azure.com/) > diretório Azure Ative > Registo de Aplicações > Selecione a sua aplicação > Proprietários > Adicionar Proprietários</span><span class="sxs-lookup"><span data-stu-id="69f37-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="69f37-111">**Não é possível ver a sua aplicação na lâmina de Registos de Aplicações, mesmo que seja o proprietário dessa aplicação?**</span><span class="sxs-lookup"><span data-stu-id="69f37-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="69f37-112">O proprietário de uma aplicação não é um papel administrativo.</span><span class="sxs-lookup"><span data-stu-id="69f37-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="69f37-113">Se a definição Restringir o [acesso ao portal de administração AD do Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) está ativado, apenas a administração poderá visualizar as aplicações no portal de Registo de Aplicações.</span><span class="sxs-lookup"><span data-stu-id="69f37-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="69f37-114">Para que um proprietário possa visualizar as aplicações, desative esta definição (Defina isto para NO) ou atribua função de administração ao proprietário apenas para a aplicação específica.</span><span class="sxs-lookup"><span data-stu-id="69f37-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="69f37-115">No entanto, você vai precisar de uma licença Azure AD Premium P2 e ativar [a Gestão de Identidade Privilegiada.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="69f37-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
