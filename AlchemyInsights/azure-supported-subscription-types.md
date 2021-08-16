---
title: Tipos de subscrição suportados
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072171"
---
# <a name="supported-subscription-types"></a>Tipos de subscrição suportados

Reveja os tipos de subscrição suportados para continuar.

[Tipos de subscrição suportados](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transferir a propriedade da faturação**

Portal do Azure como [Administrador da conta](https://ms.portal.azure.com/) da conta de faturação que tem a subscrição que pretende transferir

- Procurar **Gestão de Custos + Faturação**. Selecionar **Subscrições** no painel à esquerda. Por depender do acesso, poderá ser necessário selecionar um âmbito de faturação e depois **Subscrições** ou **subscrições Azure**.
- Selecione Transferir propriedade de faturação para a subscrição que pretende transferir.
- Introduza o endereço de e-mail de um utilizador que é administrador de faturação da conta que será o novo proprietário para a subscrição e depois selecione **enviar pedido de transferência**.
- O utilizador recebe um e-mail com instruções para rever o seu pedido de transferência. Para aprovar o pedido de transferência, o utilizador seleciona o link no e-mail e segue as instruções.

Nota: se transferir a propriedade de faturação da sua subscrição para a conta de um utilizador noutro inquilino da Microsoft Azure AD, todas atribuições de [controlo de acesso baseado em funções (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerir recursos na subscrição são permanentemente removidas. Apenas o novo proprietário terá acesso para gerir os recursos na subscrição. Para mais informações, consulte [Transferir subscrição para um utilizador noutro inquilino da Microsoft Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Transferir propriedade da subscrição**

A Transferência da Propriedade da Subscrição requer previamente que o acesso baseado na função (RBAC) gira recursos na subscrição e perca o seu acesso. Para obter mais informações sobre como adicionar uma subscrição existente a um inquilino, consulte [Associar ou adicionar uma subscrição do Azure ao Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- A Transferência de Subscrição com um montante pendente existente do ciclo de faturação atual não será transferida para o novo instrumento de pagamento na nova conta. A única informação disponível para os utilizadores na nova conta é o custo do mês anterior da sua subscrição. O resto do histórico de utilização e faturação não é transferido com a subscrição.
- A transferência da propriedade de faturação das subscrições do Contrato Enterprise (EA) só é atualmente suportada no portal do Contrato Enterprise
- Transferir uma subscrição baseada em créditos, como a do Visual Studio, BizSpark e da Microsoft Partner Network para um novo utilizador requer ter uma licença de Visual Studio/Microsoft Partner Network para aceitar o pedido de transferência
- Todos os recursos, como máquinas virtuais, discos e sites, são transferidos para a nova conta sucesso. Os seguintes recursos podem ser afetados numa transferência de subscrição entre inquilinos:

**Azure AD Domain Services**

Cofres chave do Azure

- [Os utilizadores e as bases de dados relacionados com SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) podem ser afetados, especialmente se o cliente utilizar uma autenticação relacionada com o Azure Active Directory
- **Os serviços de aplicações** configurados com a autenticação do Azure Active Directory podem ser afetados
- As contas dos Serviços do **Visual Studio Team** ligadas a subscrições do Azure podem perder temporariamente o acesso quando a subscrição do Azure associada for cancelada

**Documentos recomendados**

Passos após aceitar a propriedade da faturação:

- Para manter a propriedade da faturação, mas alterar o tipo da sua subscrição, consulte: [Alterar a sua subscrição do Azure para outra oferta](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transferência de Visual Studio, Microsoft Partner Network (MPN) e subscrições Dev/Test pague remotamente](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transferir a propriedade da faturação de subscrições do Contrato Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Transferência de Propriedade FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Resolução de Problemas Questões de Transferência de propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)