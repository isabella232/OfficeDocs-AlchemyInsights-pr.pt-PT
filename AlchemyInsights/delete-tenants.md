---
title: Apagar inquilino
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564884"
---
# <a name="delete-tenant"></a><span data-ttu-id="48856-102">Apagar inquilino</span><span class="sxs-lookup"><span data-stu-id="48856-102">Delete tenant</span></span>

<span data-ttu-id="48856-103">Para eliminar um AD Azure, certifique-se:</span><span class="sxs-lookup"><span data-stu-id="48856-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="48856-104">És administrador global no diretório.</span><span class="sxs-lookup"><span data-stu-id="48856-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="48856-105">Não está inscrito numa conta que tenha o diretório por defeito, como contoso.onmicrosoft.com na conta de assinatura, como admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="48856-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="48856-106">Remova quaisquer aplicações ativas no diretório antes da eliminação.</span><span class="sxs-lookup"><span data-stu-id="48856-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="48856-107">Para remover aplicações ativas, navegue para os registos da App e remova as aplicações existentes.</span><span class="sxs-lookup"><span data-stu-id="48856-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="48856-108">Não existem subscrições ativas para quaisquer Serviços Microsoft Online, tais como Microsoft Azure, Office 365 ou Azure AD Premium associados no diretório.</span><span class="sxs-lookup"><span data-stu-id="48856-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="48856-109">Transfira as suas subscrições ou acelere o cancelamento de subscrições ativas através do Suporte e Faturação do Azure.</span><span class="sxs-lookup"><span data-stu-id="48856-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="48856-110">Saiba mais sobre como cancelar as assinaturas Do Office 365 e Azure.</span><span class="sxs-lookup"><span data-stu-id="48856-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="48856-111">Para obter orientações sobre a associação ou a adição de uma subscrição existente a um inquilino, consulte [Associate ou adicione uma subscrição Azure ao seu inquilino AZure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="48856-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="48856-112">Não há licença ativa.</span><span class="sxs-lookup"><span data-stu-id="48856-112">There are no Active license.</span></span> <span data-ttu-id="48856-113">Para remover licenças, consulte [como remover a licença de Remoção de Assinaturas.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)</span><span class="sxs-lookup"><span data-stu-id="48856-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="48856-114">Não existem outros utilizadores ativos no diretório além de si mesmo como Administrador Global ao tentar eliminar o AD Azure.</span><span class="sxs-lookup"><span data-stu-id="48856-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="48856-115">Remova quaisquer outros utilizadores ativos, e quaisquer dependências de um nome de domínio personalizado no inquilino também terão de ser removidas, como os utilizadores criados com admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="48856-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="48856-116">Para mais detalhes, como:</span><span class="sxs-lookup"><span data-stu-id="48856-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="48856-117">Eliminar "Azure Ative Directory" ou "subscription", ver [Delete Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="48856-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="48856-118">Remover as aplicações no diretório, ver [Remoção de Aplicações](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="48856-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
