---
title: Atribuir grupos para o papel de AD Azure
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885394"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="b35c8-102">Atribuir grupos para o papel de AD Azure</span><span class="sxs-lookup"><span data-stu-id="b35c8-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="b35c8-103">Para atribuir um grupo AD Azure com fonte de autoridade em Azure AD a um papel de AD Azure, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="b35c8-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="b35c8-104">Criar um novo grupo - Criar um novo grupo:</span><span class="sxs-lookup"><span data-stu-id="b35c8-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="b35c8-105">a.</span><span class="sxs-lookup"><span data-stu-id="b35c8-105">a.</span></span> <span data-ttu-id="b35c8-106">Inscreva-se no centro de administração Azure AD com **funções privilegiadas de administrador** ou permissões **globais de administrador.**</span><span class="sxs-lookup"><span data-stu-id="b35c8-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="b35c8-107">b.</span><span class="sxs-lookup"><span data-stu-id="b35c8-107">b.</span></span> <span data-ttu-id="b35c8-108">Selecione **Azure Ative Directory > Groups > Todos os grupos > Novo grupo**.</span><span class="sxs-lookup"><span data-stu-id="b35c8-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="b35c8-109">c.</span><span class="sxs-lookup"><span data-stu-id="b35c8-109">c.</span></span> <span data-ttu-id="b35c8-110">Criar o grupo.</span><span class="sxs-lookup"><span data-stu-id="b35c8-110">Create the group.</span></span>

2. <span data-ttu-id="b35c8-111">Atribua o papel ao grupo durante a criação do grupo ou após a criação do grupo.</span><span class="sxs-lookup"><span data-stu-id="b35c8-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="b35c8-112">a.</span><span class="sxs-lookup"><span data-stu-id="b35c8-112">a.</span></span> <span data-ttu-id="b35c8-113">Para atribuir um papel ao grupo no momento da criação do grupo, ligue as **funções de AD Azure** pode ser atribuída ao grupo e criar o grupo.</span><span class="sxs-lookup"><span data-stu-id="b35c8-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="b35c8-114">b.</span><span class="sxs-lookup"><span data-stu-id="b35c8-114">b.</span></span> <span data-ttu-id="b35c8-115">Para atribuir um papel ao grupo depois de criado, navegue no separador **de funções atribuído** para o grupo recém-criado e atribua o papel ao grupo.</span><span class="sxs-lookup"><span data-stu-id="b35c8-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="b35c8-116">**Gerir a adesão a um grupo que é atribuído ao papel de Azure AD**</span><span class="sxs-lookup"><span data-stu-id="b35c8-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="b35c8-117">Para evitar a elevação de privilégios, por defeito, apenas administradores privilegiados e administradores globais podem modificar a adesão de um grupo que é atribuído a um papel.</span><span class="sxs-lookup"><span data-stu-id="b35c8-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="b35c8-118">Podem, no entanto, optar por designar um proprietário para tal grupo e delegar esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="b35c8-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="b35c8-119">Para obter mais detalhes sobre a atribuição de grupos de nuvem a funções AD Azure, consulte [atribuir uma função de AD ao Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="b35c8-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="b35c8-120">Para obter mais detalhes sobre as funções de resolução de problemas atribuídos a grupos de nuvem, consulte [as funções de resolução de problemas atribuídas a grupos de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="b35c8-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





