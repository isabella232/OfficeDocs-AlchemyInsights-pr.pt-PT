---
title: Transferir propriedade de faturação Azure
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922166"
---
# <a name="transfer-azure-billing-ownership"></a>Transferir propriedade de faturação Azure

Inscreva-se no [portal Azure](https://portal.azure.com/) como administrador da conta de faturação que tem a subscrição que pretende transferir. Se não tem a certeza se é e administrador, ou se precisa de determinar quem é, consulte [o administrador de faturação da conta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)determine .

- Pesquisa em **Gestão de Custos + Faturação.**
- Selecione **Subscrições** do painel esquerdo. Dependendo do acesso, poderá ter de selecionar um âmbito de faturação e, em seguida, **subscrições** ou **subscrições Azure**.
- **Selecione a propriedade de faturação de transferência** para a subscrição que pretende transferir
- Insira o endereço de e-mail de um utilizador que é um administrador de faturação da conta que será o novo proprietário para a subscrição e, em seguida, selecione o pedido de **transferência de envio**
- O utilizador recebe um e-mail com instruções para rever o seu pedido de transferência. Para aprovar o pedido de transferência, o utilizador seleciona o link no e-mail e segue as instruções.

**Nota:** Se transferir a propriedade da faturação da sua subscrição para a conta de um utilizador em outro inquilino da AD Azure, todas as atribuições de controlo de acesso baseado em [funções (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)para gerir recursos na subscrição são permanentemente removidas. Apenas o novo proprietário terá acesso à gestão de recursos na subscrição. Para obter mais informações, consulte [a subscrição de Transferência para um utilizador em outro inquilino AD Azure.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos Recomendados**

- [Transferir a propriedade de uma subscrição do Azure para outra conta](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Sobre a transferência de propriedade de faturação para uma subscrição do Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transfering Visual Studio, Microsoft Partner Network (MPN) e Pay à medida que vai de dev/Test subscrições](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transfer Ownership FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problemas de transferência Questões de Propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
