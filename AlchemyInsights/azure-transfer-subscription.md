---
title: Transferir a propriedade da faturação Azure
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
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755558"
---
# <a name="transfer-azure-billing-ownership"></a>Transferir a propriedade da faturação Azure

Iniciar sessão no [portal do Microsoft Azure](https://portal.azure.com/) como administrador da conta de faturação que tem a assinatura que deseja transferir. Se não tem a certeza se é um administrador, ou se precisa de determinar quem é, consulte [Determinar administrador de faturação da conta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Pesquisa sobre _Gestão de Custos + Faturação_.
1. Selecionar **Subscrições** a partir do painel da esquerda. Por depender do acesso, poderá ser necessário selecionar um âmbito de faturação e depois **Subscrições** ou **subscrições Azure**.
1. Selecione **Transferir propriedade de faturação** para a subscrição que pretende transferir.
1. Introduza o endereço de e-mail de um utilizador que é administrador de faturação da conta que será o novo proprietário para a subscrição e depois selecione **enviar pedido de transferência**.
1. O utilizador recebe um e-mail com instruções para rever o seu pedido de transferência. Para aprovar o pedido de transferência, o utilizador seleciona o link no e-mail e segue as instruções.

Note que se transferir a propriedade de faturação da sua subscrição para a conta de um utilizador noutro inquilino da Microsoft Azure Active Directory, todas [as atribuições de controlo de acesso baseado em funções (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) para gerir recursos na subscrição são permanentemente removidas. Apenas o novo proprietário terá acesso para gerir os recursos na subscrição. Para mais informações sobre como mudar de diretório para uma assinatura, ver [Transferir assinatura para um utilizador noutro inquilino da Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Impacto importante nas suas faturas**_: se transferiu a propriedade da faturação para uma subscrição Azure, os seus encargos serão pro-avaliado. Poderá aceder às faturas de acordo com o seguinte:  

1. Selecione a sua subscrição na  [página Subscrições](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal do Microsoft Azure como [um utilizador com acesso a faturas](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), depois selecione **Faturas**.
1. Clique em **Descarregar fatura** para ver uma cópia da sua fatura em PDF. Se diz _Não disponível_, ver [Porque não vejo uma fatura para o último período de faturação?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Também pode ver a sua utilização diária ao clicar no **período de faturação** para obter um PDF da sua fatura e uma cópia do seu ficheiro detalhado de utilização diária (.CSV). Para mais informações, ver [Obter dados de faturação e utilização](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documentos Recomendados**

- [Transferir a propriedade da faturação de uma subscrição Azure para outra conta](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Sobre a transferência da propriedade da faturação de uma subscrição Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transferência de Visual Studio, Microsoft Partner Network (MPN) e subscrições Dev/Test pague remotamente](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transferência de Propriedade FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Resolução de Problemas Questões de Transferência de propriedade](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
