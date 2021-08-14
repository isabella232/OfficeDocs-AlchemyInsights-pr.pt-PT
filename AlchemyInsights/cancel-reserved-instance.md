---
title: Cancelamento de reserva
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931244"
---
# <a name="cancelling-reservation"></a>Cancelamento de reserva

- **Serviço de gestão personalizada:** pode cancelar ou trocar uma instância reservada usando o [Portal do Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione a reserva e clique em reembolso ou troca. Tenha em atenção que tem de ter acesso de proprietário na ordem de reserva para proceder à troca ou reembolso. O acesso apenas à Reserva não lhe permite continuar com o reembolso ou troca. Peça ao proprietário da ordem de reserva para lhe conceder acesso de proprietário à ordem de reserva
- **Política de troca:** pode trocar uma reserva por outra reserva do mesmo tipo – não existem **penalizações** na reserva. O compromisso total com a nova reserva deve ser superior ao montante do reembolso da reserva trocada e aos pagamentos mensais futuros (se aplicável).
- **Política de reembolso:** a soma do reembolso e dos futuros pagamentos cancelados não pode exceder 50.000 $ num espaço de 12 meses consecutivos. Atualmente, **estamos a não cobrar quaisquer** penalizações sobre os reembolsos, mas podemos vir a cobrá-las em reembolsos futuros  
    **Exceções:** a funcionalidade de gestão personalizada e o cancelamento não estão disponíveis para clientes com Contrato Enterprise do Governo dos Estados Unidos
- O suporte **API / PS / CLI** não está disponível para cancelamento nem reembolsos para [Trocas de gestão personalizada e reembolsos para Reservas no Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A funcionalidade de troca e cancelamento de gestão personalizada não se encontra disponível para clientes com Contrato Enterprise do Governo dos Estados Unidos. São suportados outros tipos de subscrição do Governo dos Estados Unidos, incluindo Pay-As-You-Go e Fornecedor de Soluções em Nuvem da Microsoft

Saiba mais: [Como as transações de reembolso e de troca são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Saiba mais: [Políticas de reembolso e de troca](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Outras perguntas: [Visite documentos de instâncias reservadas](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Trocar uma instância reservada existente (serviço de gestão personalizada)**

Pode trocar uma reserva por outra reserva do mesmo tipo. Também pode reembolsar uma reserva, até 50.000 $ por ano, se já não precisar da mesma. A funcionalidade de troca e cancelamento de gestão personalizada não se encontra disponível para clientes com Contrato Enterprise do Governo dos Estados Unidos. São suportados outros tipos de subscrição do Governo dos Estados Unidos, incluindo Pay-As-You-Go e Fornecedor de Soluções em Nuvem da Microsoft. Tem de ter acesso de proprietário na ordem de reserva para proceder à troca ou reembolso de uma reserva existente.

Os passos seguintes irão guiar o procedimento para concluir a transação

1. Inicie sessão no seu [Portal do Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione as reservas que pretende reembolsar e clique em **Trocar**
2. Selecione o produto VM que pretende comprar e insira uma quantidade. Certifique-se de que o novo total da compra é superior ao total da devolução [Determine o tamanho certo antes de efetuar a compra](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Rever e concluir a transação

**Reembolso de uma instância reservada**

Para reembolsar uma reserva, aceda a **Detalhes da reserva** e clique em **Reembolso**

**Reembolso proporcional:**

**Exemplos de reembolsos proporcionais e de requisitos mínimos para reembolso e troca**  
Exemplo de reserva com antecedência:

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

**Documentos recomendados**

- [Como as transações de reembolso e de troca são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Políticas de reembolso e de troca](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)