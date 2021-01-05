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
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Como adicionar e gerir administradores - passos recomendados

Com base na descrição do seu problema, encontrámos uma solução para si. A maioria dos clientes conseguiu resolver o seu problema por conta própria depois de seguir a nossa documentação.

**Editar o Administrador de Subscrição ou Coadministrador**

- O Administrador de Conta pode editar ambas as funções, enquanto que o Administrador de Subscrição só pode alterar coadministradores no [portal Azure](https://ms.portal.azure.com/#home).
- [Adicionar ou alterar administradores de subscrição do Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Atualizar o Administrador de Subscrição ou Co-Administrator para Subscrições Internas (AIRS)**

O Administrador de Serviço ou o Coadministrador podem auto-servir esta ação utilizando os seguintes passos:

1. Faça login no [portal Azure](https://ms.portal.azure.com/#home) e clique em **Gestão de Custos + Faturação** na lâmina esquerda.
2. Clique no item da linha com a sua subscrição. Isto abre a Visão Geral para a sua subscrição.
3. Na lâmina **de subscrição,** clique em **Propriedades**. 
4. Clique no botão **Administração de Serviço.**
5. Introduza o e-mail do utilizador a quem pretende definir como Administrador de Serviço e clique **em OK**.

**Adicionar/Alterar/Remover Coadministrador**

1. Faça login no [portal Azure](https://ms.portal.azure.com/#home) como Administrador de Serviço.
2. Abrir [subscrições](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) e selecionar uma subscrição. (Os coadministradores só podem ser designados no âmbito da subscrição.)
3. Navegar para **o controlo de acesso (IAM)** Administradores  >  **clássicos**  >  **Add**  >  **Add coadministrador** para abrir o painel de **coadministração Add** (Se a opção de coadministrador Add estiver desativada, denota que não tem permissões).
4. Selecione o utilizador a quem pretende adicionar e clique em **Adicionar**.

**Saiba mais:**
- [Adicionar um Coadministrador](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Remover um coadministrador](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Alterar o Administrador de Serviço](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ver o Administrador de Conta](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gerir o acesso através do portal RBAC e Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Adicionar/eliminar utilizadores usando O Diretório Ativo Azure (AD)**

Pode adicionar novos utilizadores ou eliminar os utilizadores existentes da sua organização Azure Ative Directory (Azure AD):

1. Para adicionar um novo utilizador, inicie sessão no [portal Azure](https://ms.portal.azure.com/#home) como administrador do Utilizador para a organização.
2. Selecione **Azure Ative Directory**, selecione **Utilizadores** e, em seguida, clique em **Novo utilizador**.
3. Na página **do Utilizador,** preencha as informações necessárias. Clique **em Criar**. O utilizador é criado e adicionado ao seu inquilino Azure AD.

**Saiba mais:**

- [Adicionar um novo utilizador](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Eliminar um utilizador](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Adicionar ou atualizar as informações de perfil de um utilizador utilizando o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documentos recomendados**

- [O que é o controlo de acesso baseado em funções (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Compreender os diferentes papéis em Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Permissões de funções de administrador no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Tutorial: Conceder acesso a um utilizador que utilize o RBAC e o portal Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Resolução de problemas RBAC em Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organize os seus recursos com grupos de gestão Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Como solicitar cópia da fatura da Azure por e-mail](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Como adicionar, atualizar ou remover um cartão de crédito ou débito da Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gerir (Reativar/Cancelar/Trocar) subscrição](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



