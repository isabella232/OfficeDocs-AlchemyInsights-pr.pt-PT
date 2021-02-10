---
title: Gerir uma identidade gerida atribuída pelo utilizador
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177773"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="c086c-102">Gerir uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="c086c-103">A gestão de uma identidade gerida atribuída pelo utilizador implica:</span><span class="sxs-lookup"><span data-stu-id="c086c-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="c086c-104">Atribuir funções a uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="c086c-105">Eliminação de uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="c086c-106">Listagem de uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="c086c-107">Para obter mais informações sobre as tarefas acima mencionadas, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="c086c-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="c086c-108">[Como criar uma identidade gerida atribuída pelo utilizador](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - para atribuir funções a uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="c086c-109">[Como eliminar uma identidade gerida atribuída pelo utilizador](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - para eliminar uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="c086c-110">[Como listar uma identidade gerida atribuída pelo utilizador](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - para listar uma identidade gerida atribuída pelo utilizador</span><span class="sxs-lookup"><span data-stu-id="c086c-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="c086c-111">Verifique se tem a atribuição **de função de Contribuinte de Identidade Gerida.**</span><span class="sxs-lookup"><span data-stu-id="c086c-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="c086c-112">Esta atribuição de funções é necessária para criar/eliminar identidades geridas atribuídas pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="c086c-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
