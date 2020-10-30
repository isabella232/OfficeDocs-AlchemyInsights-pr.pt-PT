---
title: Tipos de subscrição suportados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807976"
---
# <a name="supported-subscription-types"></a>Tipos de subscrição suportados

Por favor, reveja os tipos de subscrição suportados para prosseguir.

[Tipos de subscrição suportados](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Propriedade de faturação de transferência**

Portal Azure como [Admin conta](https://ms.portal.azure.com/) da conta de faturação que tem a subscrição que pretende transferir

- Pesquisa em **Gestão de Custos + Faturação.** Selecione **Subscrições** do painel esquerdo. Dependendo do acesso, poderá ter de selecionar um âmbito de faturação e, em seguida, **subscrições** ou **subscrições Azure** .
- Selecione a propriedade de faturação de transferência para a subscrição que pretende transferir
- Insira o endereço de e-mail de um utilizador que é um administrador de faturação da conta que será o novo proprietário para a subscrição e, em seguida, selecione o pedido de **transferência de envio**
- O utilizador recebe um e-mail com instruções para rever o seu pedido de transferência. Para aprovar o pedido de transferência, o utilizador seleciona o link no e-mail e segue as instruções.

Nota: Se transferir a propriedade da faturação da sua subscrição para a conta de um utilizador em outro inquilino da AD Azure, todas as atribuições de controlo de acesso baseado em [funções (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerir recursos na subscrição são permanentemente removidas. Apenas o novo proprietário terá acesso à gestão de recursos na subscrição. Para obter mais informações, consulte [a subscrição de Transferência para um utilizador em outro inquilino AD Azure.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Propriedade de Transferência de Subscrição**

A Subscrição Ownership Transfer pré-requisitos de acesso baseado em funções (RBAC) para gerir os recursos na subscrição perde o seu acesso. Para obter mais informações sobre a adição de uma subscrição existente a um inquilino, consulte [Associate ou adicione uma subscrição Azure ao Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- A Transferência de Assinaturas com um montante em dívida existente do ciclo de faturação em curso não será transferida para o novo instrumento de pagamento na nova conta. A única informação disponível para os utilizadores em nova conta é o custo do último mês para a sua subscrição. O resto do histórico de utilização e faturação não transfere com a subscrição.
- A propriedade de faturação de transferência de subscrições do Acordo Empresarial (EA) é atualmente suportada apenas no Portal do Acordo Empresarial
- Transferir uma subscrição orientada para o crédito como Visual Studio, BizSpark, Microsoft Partner Network para um novo utilizador requer ter uma licença de rede de parceiros Visual Studio/Microsoft para aceitar o pedido de transferência
- Todos os recursos como Máquinas Virtuais, discos e websites transferem-se para a nova conta com sucesso. Os seguintes recursos podem ser afetados numa transferência de assinatura de inquilinos cruzados:

**Serviços de domínio Azure Ad**

Cofres de chaves Azure

- [Os utilizadores e bases de dados relacionados com](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) o SQL podem ser impactados, especialmente se o cliente utilizar uma autenticação relacionada com o Azure Ative Directory
- **Serviços de aplicações** configurados com autenticação do Azure Ative Directory podem ser impactados
- **Equipa visual de estúdio** As contas de serviços ligadas às subscrições do Azure podem perder temporariamente o acesso quando a subscrição do Azure conectada for cancelada

**Documentos Recomendados**

Passos após a aceitação da propriedade da faturação:

- Para manter a propriedade de faturação, mas alterar o tipo de subscrição, consulte: [Mude a sua subscrição Azure para outra oferta](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transfering Visual Studio, Microsoft Partner Network (MPN) e Pay à medida que vai de dev/Test subscrições](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Propriedade de faturação de transferência de assinaturas do Acordo Empresarial (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Transfer Ownership FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problemas de transferência Questões de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)