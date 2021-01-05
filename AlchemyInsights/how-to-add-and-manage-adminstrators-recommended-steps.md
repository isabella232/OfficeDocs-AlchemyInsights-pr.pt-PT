---
title: Como adicionar e gerir administradores - passos recomendados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755846"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="72a53-102">Como adicionar e gerir administradores - passos recomendados</span><span class="sxs-lookup"><span data-stu-id="72a53-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="72a53-103">Com base na descrição do seu problema, encontrámos uma solução para si.</span><span class="sxs-lookup"><span data-stu-id="72a53-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="72a53-104">A maioria dos clientes conseguiu resolver o seu problema por conta própria depois de seguir a nossa documentação.</span><span class="sxs-lookup"><span data-stu-id="72a53-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="72a53-105">**Editar o Administrador de Subscrição ou Coadministrador**</span><span class="sxs-lookup"><span data-stu-id="72a53-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="72a53-106">O Administrador de Conta pode editar ambas as funções, enquanto que o Administrador de Subscrição só pode alterar coadministradores no [portal Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="72a53-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="72a53-107">Adicionar ou alterar administradores de subscrição do Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="72a53-108">**Atualizar o Administrador de Subscrição ou Co-Administrator para Subscrições Internas (AIRS)**</span><span class="sxs-lookup"><span data-stu-id="72a53-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="72a53-109">O Administrador de Serviço ou o Coadministrador podem auto-servir esta ação utilizando os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="72a53-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="72a53-110">Faça login no [portal Azure](https://ms.portal.azure.com/#home) e clique em **Gestão de Custos + Faturação** na lâmina esquerda.</span><span class="sxs-lookup"><span data-stu-id="72a53-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="72a53-111">Clique no item da linha com a sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="72a53-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="72a53-112">Isto abre a Visão Geral para a sua subscrição.</span><span class="sxs-lookup"><span data-stu-id="72a53-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="72a53-113">Na lâmina **de subscrição,** clique em **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="72a53-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="72a53-114">Clique no botão **Administração de Serviço.**</span><span class="sxs-lookup"><span data-stu-id="72a53-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="72a53-115">Introduza o e-mail do utilizador a quem pretende definir como Administrador de Serviço e clique **em OK**.</span><span class="sxs-lookup"><span data-stu-id="72a53-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="72a53-116">**Adicionar/Alterar/Remover Coadministrador**</span><span class="sxs-lookup"><span data-stu-id="72a53-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="72a53-117">Faça login no [portal Azure](https://ms.portal.azure.com/#home) como Administrador de Serviço.</span><span class="sxs-lookup"><span data-stu-id="72a53-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="72a53-118">Abrir [subscrições](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selecionar uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="72a53-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="72a53-119">(Os coadministradores só podem ser designados no âmbito da subscrição.)</span><span class="sxs-lookup"><span data-stu-id="72a53-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="72a53-120">Navegar para **o controlo de acesso (IAM)** Administradores  >  **clássicos**  >  **Add**  >  **Add coadministrador** para abrir o painel de **coadministração Add** (Se a opção de coadministrador Add estiver desativada, denota que não tem permissões).</span><span class="sxs-lookup"><span data-stu-id="72a53-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="72a53-121">Selecione o utilizador a quem pretende adicionar e clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="72a53-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="72a53-122">**Saiba mais:**</span><span class="sxs-lookup"><span data-stu-id="72a53-122">**Learn more:**</span></span>
- [<span data-ttu-id="72a53-123">Adicionar um Coadministrador</span><span class="sxs-lookup"><span data-stu-id="72a53-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="72a53-124">Remover um coadministrador</span><span class="sxs-lookup"><span data-stu-id="72a53-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="72a53-125">Alterar o Administrador de Serviço</span><span class="sxs-lookup"><span data-stu-id="72a53-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="72a53-126">Ver o Administrador de Conta</span><span class="sxs-lookup"><span data-stu-id="72a53-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="72a53-127">Gerir o acesso através do portal RBAC e Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="72a53-128">**Adicionar/eliminar utilizadores usando O Diretório Ativo Azure (AD)**</span><span class="sxs-lookup"><span data-stu-id="72a53-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="72a53-129">Pode adicionar novos utilizadores ou eliminar os utilizadores existentes da sua organização Azure Ative Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="72a53-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="72a53-130">Para adicionar um novo utilizador, inicie sessão no [portal Azure](https://ms.portal.azure.com/#home) como administrador do Utilizador para a organização.</span><span class="sxs-lookup"><span data-stu-id="72a53-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="72a53-131">Selecione **Azure Ative Directory**, selecione **Utilizadores** e, em seguida, clique em **Novo utilizador**.</span><span class="sxs-lookup"><span data-stu-id="72a53-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="72a53-132">Na página **do Utilizador,** preencha as informações necessárias.</span><span class="sxs-lookup"><span data-stu-id="72a53-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="72a53-133">Clique **em Criar**.</span><span class="sxs-lookup"><span data-stu-id="72a53-133">Click **Create**.</span></span> <span data-ttu-id="72a53-134">O utilizador é criado e adicionado ao seu inquilino Azure AD.</span><span class="sxs-lookup"><span data-stu-id="72a53-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="72a53-135">**Saiba mais:**</span><span class="sxs-lookup"><span data-stu-id="72a53-135">**Learn more**:</span></span>

- [<span data-ttu-id="72a53-136">Adicionar um novo utilizador</span><span class="sxs-lookup"><span data-stu-id="72a53-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="72a53-137">Eliminar um utilizador</span><span class="sxs-lookup"><span data-stu-id="72a53-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="72a53-138">Adicionar ou atualizar as informações de perfil de um utilizador utilizando o Azure Ative Directory</span><span class="sxs-lookup"><span data-stu-id="72a53-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="72a53-139">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="72a53-139">**Recommended documents**</span></span>

- [<span data-ttu-id="72a53-140">O que é o controlo de acesso baseado em funções (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="72a53-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="72a53-141">Compreender os diferentes papéis em Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="72a53-142">Permissões de funções de administrador no Azure Ative Directory</span><span class="sxs-lookup"><span data-stu-id="72a53-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="72a53-143">Tutorial: Conceder acesso a um utilizador que utilize o RBAC e o portal Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="72a53-144">Resolução de problemas RBAC em Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="72a53-145">Organize os seus recursos com grupos de gestão Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="72a53-146">Como solicitar cópia da fatura da Azure por e-mail</span><span class="sxs-lookup"><span data-stu-id="72a53-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="72a53-147">Como adicionar, atualizar ou remover um cartão de crédito ou débito da Azure</span><span class="sxs-lookup"><span data-stu-id="72a53-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="72a53-148">Gerir (Reativar/Cancelar/Trocar) subscrição</span><span class="sxs-lookup"><span data-stu-id="72a53-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



