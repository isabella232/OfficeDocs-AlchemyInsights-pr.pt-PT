---
title: Cancelamento de reserva
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807993"
---
# <a name="cancelling-reservation"></a>Cancelamento de reserva

- **Self-service:** Pode cancelar ou trocar uma instância reservada usando o [portal Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selecione a reserva e clique em reembolso ou troca. Note que deve ter acesso ao proprietário na Ordem de Reserva para trocar ou reembolsar. O acesso apenas à Reserva não o permitirá proceder com reembolso ou troca. Peça ao proprietário da Ordem de Reserva para lhe dar acesso ao proprietário à Ordem de Reserva
- **Política de câmbio:** Pode trocar uma reserva por outra reserva do mesmo tipo – **não existem sanções** na troca de reservas. O compromisso total com nova reserva deve ser superior à soma do montante de reembolso da reserva trocada e dos pagamentos mensais futuros (se aplicável)
- **Política de reembolso:** A soma do reembolso e os pagamentos futuros cancelados não podem exceder $50.000 USD numa janela de 12 meses. Neste **momento, não estamos a cobrar qualquer penalidade** sobre reembolsos, mas podemos cobrar-lhe reembolsos futuros.  
    **Exceções:** A capacidade de troca de self-service e de cancelamento não está disponível para clientes do Acordo Empresarial do Governo dos EUA
- O suporte **da API / PS/CLI** não está disponível para cancelamento e reembolsos [trocas de self-service e reembolsos para Reservas Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- A capacidade de troca de self-service e cancelamento não está disponível para clientes do Acordo Empresarial do Governo dos EUA. Outros tipos de subscrição do Governo dos EUA, incluindo Pay-As-You-Go e CSP são apoiados

Saiba mais: [Como as transações de retorno e de troca são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Saiba mais: [Políticas de troca e reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Outras questões: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Troque uma instância reservada existente (Self-service)**

Pode trocar uma reserva por outra reserva do mesmo tipo. Você também pode reembolsar uma reserva, até $50.000 USD por ano, se você não precisar mais. A capacidade de troca de self-service e cancelamento não está disponível para clientes do Acordo Empresarial do Governo dos EUA. Outros tipos de subscrição do Governo dos EUA, incluindo Pay-As-You-Go e CSP, são apoiados. Deve ter acesso ao proprietário na Ordem de Reserva para trocar ou reembolsar uma reserva existente.

As seguintes etapas orientarão o procedimento para concluir a transação

1. Faça login no seu [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selecione as reservas que pretende reembolsar e clique em **Trocar**
2. Selecione o produto VM que pretende comprar e digite uma quantidade. Certifique-se de que o novo total de compras é mais do que o total de retorno [Determinar o tamanho certo antes de comprar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Rever e concluir a transação

**Reembolso por instância reservada**

Para reembolsar uma reserva, vá a **Detalhes da Reserva** e clique em **Reembolsar**

**Reembolso pro-nominal:**

**Pró-ração e mínimos de requisitos para reembolso e troca**  
Exemplo de reserva inicial:

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

**Documentos Recomendados**

- [Como as transações de devolução e de câmbio são processadas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Políticas de troca e reembolso](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)