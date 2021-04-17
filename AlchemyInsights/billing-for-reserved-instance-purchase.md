---
title: Faturação para compra de Instância Reservada
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820333"
---
# <a name="billing-for-reserved-instance-purchase"></a>Faturação para compra de Instância Reservada

A compra de instância reservada é cobrada ao método de pagamento ligado à subscrição que seleciona no momento da compra. O tipo de subscrição deve ser um acordo de empresa (número de oferta: MS-AZR-0017P), Pay-As-You-Go (número de oferta: MS-AZR-0003P), Microsoft Customer Agreement ou CSP.

- Para uma subscrição de empresa, os encargos são deduzidos do saldo de compromisso monetário da inscrição ou cobrados como overage
- Para a subscrição Pay-As-You-Go, os encargos são cobrados no cartão de crédito ou no método de pagamento da fatura na subscrição

**Cancelamento de reserva**

- **Self-service:** Pode cancelar ou trocar uma instância reservada usando o [portal Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecione a reserva e clique em reembolso ou troca. Note que deve ter acesso ao proprietário na Ordem de Reserva para trocar ou reembolsar. O acesso apenas à Reserva não o permitirá proceder com reembolso ou troca. Peça ao proprietário da Ordem de Reserva para lhe dar acesso ao proprietário à Ordem de Reserva
- **Política de câmbio:** Pode trocar uma reserva por outra reserva do mesmo tipo – **não existem sanções** na troca de reservas. O compromisso total com nova reserva deve ser superior à soma do montante de reembolso da reserva trocada e dos pagamentos mensais futuros (se aplicável)
- **Política de reembolso:** A soma do reembolso e os pagamentos futuros cancelados não podem exceder $50.000 USD numa janela de 12 meses. Neste **momento, não estamos a cobrar qualquer penalidade** sobre reembolsos, mas podemos cobrar-lhe reembolsos futuros.

**Exceções:** A capacidade de troca de self-service e de cancelamento não está disponível para clientes do Acordo Empresarial do Governo dos EUA

- O suporte **da API / PS/CLI** não está disponível para cancelamento e reembolsos [trocas de self-service e reembolsos para Reservas Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A capacidade de troca de self-service e cancelamento não está disponível para clientes do Acordo Empresarial do Governo dos EUA. Outros tipos de subscrição do Governo dos EUA, incluindo Pay-As-You-Go e CSP são apoiados

Saiba mais: [Como as transações de devolução e troca são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Saiba mais: [Políticas de troca e reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Outras questões: Visite os [docs de instância reservados](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Troque uma instância reservada existente (Self-service)**

Pode trocar uma reserva por outra reserva do mesmo tipo. Você também pode reembolsar uma reserva, até $50.000 USD por ano, se você não precisar mais. A capacidade de troca de self-service e cancelamento não está disponível para clientes do Acordo Empresarial do Governo dos EUA. Outros tipos de subscrição do Governo dos EUA, incluindo Pay-As-You-Go e CSP, são apoiados. Deve ter acesso ao proprietário na Ordem de Reserva para trocar ou reembolsar uma reserva existente.

As seguintes etapas orientarão o procedimento para concluir a transação

1.Faça login no seu [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione as reservas que pretende reembolsar e clique em **Exchange** 2.Selecione o produto VM que pretende comprar e digite uma quantidade. Certifique-se de que o novo total de compra é mais do que o total de retorno [Determinar o tamanho certo antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Rever e concluir a transação

**Reembolso por instância reservada**

Para reembolsar uma reserva, vá a **Detalhes da Reserva** e clique em **Reembolsar**

**Reembolso pro-nominal:**

**Pró-ração e mínimos de requisitos para reembolso e troca** Exemplo de reserva inicial:

- Você compra um termo de um ano RI por $120 no dia 1 de janeiro
- No dia 7 de abril você quer reembolsar ou trocar esta reserva
- Uma vez que a reserva está ao vivo há 97 dias, você receberá (1-97/365) * $120 de volta. (ou seja, $88.1). Atualmente, não existe qualquer penalização sobre reembolsos
- Se trocar, a sua nova compra deve ser superior a $88.1
- Não há nenhuma penalidade sobre reembolsos atualmente

**Exemplo de reserva do plano de faturação:**

- Compra-se um ri de um ano por $10 por mês
- No dia 7 de abril você quer reembolsar ou trocar esta reserva
- Uma vez que o último pagamento aconteceu 7 dias, você receberá (1-7/31) * $10 de volta. (ou seja, $7,74)
- Os pagamentos futuros cancelados são $80. Atualmente, não existe qualquer penalização sobre reembolsos
- Este cancelamento irá deduzir $87.74 de você é o limite de reembolso de $50.000
- Se trocar, o valor total da nova compra deve ser superior a $87.74

**Não pode ver fatura para o último período de faturação**

Algumas razões possíveis para não ver uma fatura:

- Tem um valor de crédito mensal com a sua subscrição que não excedeu ou tem um Teste Gratuito. Uma fatura só é gerada quando se deve dinheiro
- Falta menos de 30 dias para o dia em que subscreveu o Azure.
- A fatura ainda não foi gerada. Aguarde até ao fim do período de faturação
- Se não for o Administrador de Conta, as faturas mais antigas podem não estar disponíveis para si

**Faça o download da sua fatura do portal Azure (.pdf)**

- Selecione a sua subscrição a partir da página [subscrições](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal Azure como [um utilizador com acesso a faturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selecione **Faturas**
- Clique **em Baixar Fatura** para ver uma cópia da sua fatura PDF. Se diz **não disponível,** veja [por que não vejo uma fatura para o último período de faturação?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Receba a sua fatura por e-mail (.pdf)**

- Selecione a sua subscrição na página [De Subscrições.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Clique **em Faturas** e envie por email a minha fatura
- Clique **em optar** e aceitar os termos. Terá de optar por cada subscrição que possuir

Nota: Se não receber um e-mail depois de seguir os passos, certifique-se de que o seu endereço de e-mail está correto nas preferências de [comunicação do seu perfil](https://account.windowsazure.com/profile)

**Descarregue os seus dados de utilização a partir do portal Azure**

- Inscreva-se no [Centro de Contas Azure](https://account.windowsazure.com/Subscriptions) como Administrador [de Conta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selecione a subscrição para a qual deseja a fatura e informações de utilização
- Selecione **História de Faturação**
- Selecione **'Ouvir a Declaração Actual'** para ver uma estimativa dos seus encargos no momento em que a estimativa foi gerada
- Selecione **Baixar o Uso** para descarregar os dados de utilização diária como um ficheiro CSV. Se vir duas versões disponíveis, baixe a versão 2

Outras questões: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos Recomendados**

- [Básicos de faturação](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entenda como é aplicado o desconto de Instância Reservada](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Faça o download ou veja a sua faturação Azure e dados de utilização diários](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Entenda como é aplicado o desconto de Instância Reservada](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender o uso de Instância Reservada para a sua subscrição Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender o uso de Instância Reservada para a sua inscrição na Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Custos de software do Windows não incluídos em instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instâncias reservadas no programa Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)