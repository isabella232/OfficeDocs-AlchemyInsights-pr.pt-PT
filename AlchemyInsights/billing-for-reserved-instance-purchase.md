---
title: Faturação da compra da Instância Reservada
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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104031"
---
# <a name="billing-for-reserved-instance-purchase"></a>Faturação da compra da Instância Reservada

A compra da instância reservada é debitada no método de pagamento associado à subscrição que selecionou no momento da compra. O tipo de subscrição tem de ser um contrato enterprise (número da oferta: MS-AZR-0017P), Pay As You Go (número da oferta: MS-AZR-0003P), Contrato de Cliente Microsoft ou CSP.

- No caso de uma subscrição empresarial, os encargos são deduzidos do saldo da alocação monetária da inscrição ou cobrados enquanto excesso
- No caso da subscrição Pay As You Go, os encargos são faturados no cartão de crédito ou método de pagamento da fatura na subscrição

**Cancelamento de reserva**

- **Serviço de gestão personalizada:** pode cancelar ou trocar uma instância reservada usando o [Portal do Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione a reserva e clique em reembolso ou troca. Tenha em atenção que tem de ter acesso de proprietário na ordem de reserva para proceder à troca ou reembolso. O acesso apenas à Reserva não lhe permite continuar com o reembolso ou troca. Peça ao proprietário da ordem de reserva para lhe conceder acesso de proprietário à ordem de reserva
- **Política de troca:** pode trocar uma reserva por outra reserva do mesmo tipo – não existem **penalizações** na reserva. O compromisso total com a nova reserva deve ser superior ao montante do reembolso da reserva trocada e aos pagamentos mensais futuros (se aplicável).
- **Política de reembolso:** a soma do reembolso e dos futuros pagamentos cancelados não pode exceder 50.000 $ num espaço de 12 meses consecutivos. Atualmente, **estamos a não cobrar quaisquer** penalizações sobre os reembolsos, mas podemos vir a cobrá-las em reembolsos futuros

**Exceções:** a funcionalidade de gestão personalizada e o cancelamento não estão disponíveis para clientes com Contrato Enterprise do Governo dos Estados Unidos

- O suporte **API / PS / CLI** não está disponível para cancelamento nem reembolsos para [Trocas de gestão personalizada e reembolsos para Reservas no Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A funcionalidade de troca e cancelamento de gestão personalizada não se encontra disponível para clientes com Contrato Enterprise do Governo dos Estados Unidos. São suportados outros tipos de subscrição do Governo dos Estados Unidos, incluindo Pay-As-You-Go e Fornecedor de Soluções em Nuvem da Microsoft

Saiba mais: [Como são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) as transações de devolução e de troca Saiba mais [:](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Exchange e Políticas de reembolso Outras perguntas: Visitar documentos de [instância reservada](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Trocar uma instância reservada existente (serviço de gestão personalizada)**

Pode trocar uma reserva por outra reserva do mesmo tipo. Também pode reembolsar uma reserva, até 50.000 $ por ano, se já não precisar da mesma. A funcionalidade de troca e cancelamento de gestão personalizada não se encontra disponível para clientes com Contrato Enterprise do Governo dos Estados Unidos. São suportados outros tipos de subscrição do Governo dos Estados Unidos, incluindo Pay-As-You-Go e Fornecedor de Soluções em Nuvem da Microsoft. Tem de ter acesso de proprietário na ordem de reserva para proceder à troca ou reembolso de uma reserva existente.

Os passos seguintes irão guiar o procedimento para concluir a transação

1. Instrua sessão no [seu portal do Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione as reservas que pretende reembolsar e **clique Exchange** 2.Selecione o produto de VM que pretende comprar e escreva uma quantidade. Certifique-se de que o novo total de compra é mais do que o total de devolução [Determinar o tamanho certo antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Rever e concluir a transação

**Reembolso de uma instância reservada**

Para reembolsar uma reserva, aceda a **Detalhes da reserva** e clique em **Reembolso**

**Reembolso proporcional:**

**Pro de migração e requisitos mínimos para reembolso e troca** Exemplo de reserva antecipada:

- Compra um termo de RI de um ano por 120 $ em 1 de janeiro
- Em 7 de abril deseja reembolsar ou trocar esta reserva
- Como a reserva se encontra ativa há 97 dias, receberá (1-97/365) * 120$ de volta. (por exemplo, 88,1$). Neste momento, não existe nenhuma penalização sobre reembolsos
- Se trocar, a sua nova compra deve ser superior a 88,1$
- Neste momento, não existe nenhuma penalização sobre reembolsos

**Exemplo de reserva de plano de faturação:**

- Compra um termo de RI de um ano por 10 $ por mês
- Em 7 de abril deseja reembolsar ou trocar esta reserva
- Como o último pagamento ocorreu há 7 dias, receberá (1-7/31) *10 $ de volta. (por exemplo, 7,74$)
- Os pagamentos futuros cancelados são de 80 $. Neste momento, não existe nenhuma penalização sobre reembolsos
- Este cancelamento irá deduzir 87,74$ do limite de reembolso de 50.000$
- Se trocar, o valor total da sua nova compra deve ser superior a 87,74$

**Não é possível ver a fatura do último período de faturação**

Eis algumas razões possíveis para não ver uma fatura:

- Tem um montante de crédito mensal com a sua subscrição que não excedeu ou que tem uma Avaliação Gratuita. Uma fatura só é gerada quando deve dinheiro
- São menos de 30 dias após o dia em que subscreveu o Azure
- A fatura ainda não foi gerada. Aguarde até ao fim do período de faturação
- Se não for o Administrador de Conta, as faturas mais antigas poderão não estar disponíveis para si

**Transferir a sua fatura a partir do portal do Azure (.pdf)**

- Selecione a sua subscrição a partir da [página Subscrições](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) no portal do Azure como [utilizador com acesso a faturas](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Selecione Faturas**
- Clique em **Transferir fatura** para ver uma cópia da sua fatura em PDF. Se disser **Indisponível**, veja [Porque não vejo uma fatura para o último período de faturação?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).

**Receber a sua fatura por e-mail (.pdf)**

- Selecione a sua [subscrição na página Subscrições.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Clique em **Faturas e, em** seguida, em Enviar a minha fatura por e-mail
- Clique **em optar ativos** e aceite os termos. Terá de optar ativamente por ativar por cada subscrição que possuir

Nota: se não receber um e-mail após seguir os passos, certifique-se de que o seu endereço de e-mail está correto nas [preferências](https://account.windowsazure.com/profile) de comunicação no seu perfil

**Transferir os seus dados de utilização a partir do portal do Azure**

- Inscreva-se [no Centro de Conta do Azure](https://account.windowsazure.com/Subscriptions) como Administrador de [Conta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selecione a subscrição para a qual pretende obter a fatura e as informações de utilização
- Selecione **Histórico de Faturação**
- **Selecione Ver Declaração** Atual para ver uma estimativa dos seus encargos no momento em que a estimativa foi gerada
- **Selecione Transferir Utilização** para transferir os dados de utilização diária como um ficheiro CSV. Se vir duas versões disponíveis, transfira a versão 2

Outras perguntas: [Visite documentos de instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documentos recomendados**

- [Noções básicas de faturação](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender como o desconto da Instância Reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transferir ou ver a sua fatura do Azure e os dados de utilização diária](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender como o desconto da Instância Reservada é aplicado](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender a utilização da Instância Reservada para a sua subscrição do Pay-As-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Compreender a utilização da Instância Reservada para a sua inscrição Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows de software não incluídos em instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instâncias Reservadas no programa Partner Central Fornecedor de Soluções em Nuvem (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)