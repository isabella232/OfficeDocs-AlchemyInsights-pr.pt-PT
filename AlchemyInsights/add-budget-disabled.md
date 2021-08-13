---
title: Porque está o botão Adicionar orçamento desativado para mim?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954687"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Porque está o botão Adicionar orçamento desativado para mim?

Para criar um orçamento, precisa de uma das seguintes permissões:

- Grupo de Gestão, Subscrição, Âmbitos de Grupos de Recursos
- Contribuinte da Gestão de Custos
- Proprietário
- Contribuinte
- Apenas Para Clientes Empresariais: Inscrição, Departamento, Âmbitos da Conta
- Administrador de Inscrição (definir orçamento no âmbito Inscrição)
- Administrador do Departamento (definir orçamento no âmbito Departamento)
- Proprietário da Conta (definir orçamento no âmbito conta)
- Apenas Contrato de Cliente Moderno: Conta de Faturação, Perfil de Faturação, Âmbitos da Secção Fatura
- Criador de subscrições do Azure

**Criei um orçamento quando o meu custo do mês atual já excedia o orçamento. Por que motivo não recebi um alerta?**  
Se já tiver excedido um determinado limite de custos ao criar um orçamento que não será atedido. Quando um novo ciclo começar, se violar o limiar, o alerta será ateado.

**Quando devo esperar receber um alerta depois de exceder um dos meus limiares de alerta de orçamento definidos?**  
Os orçamentos são avaliados a cada 4 horas. Os dados de utilização demoram pelo menos 8 horas a chegar ao sistema de orçamentos. Dado isto, os alertas podem demorar até 12 horas a ser incendiados depois de exceder um limite.

**Porque é que o botão Data de início está desativado quando seleciono um período de reposição de Mês ou Mês de faturação?**  
Os orçamentos estão alinhados com o mês do calendário atual ou com o período de faturação atual (no caso em que o Mês de Faturação está selecionado). Por este motivo, preenchimos este valor automaticamente.

**Por que motivo não vejo um gráfico dos meus custos na experiência de criação de orçamento?**  
Precisamos de um mínimo de 2 meses de dados de custos antes de podermos criar um gráfico para o ajudar na criação de orçamentos.

**Por que motivo não consigo definir um orçamento para uma subscrição que acabei de criar?**  
Após a criação de uma subscrição, os dados demoram 24 a 48 horas a processar antes de definir um orçamento para a mesma.

**Recursos da API Do Orçamento**

- [API de Orçamentos v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)fornece operações para criar e atualizar orçamentos. Ao utilizar a API de Orçamentos, pode definir um limite de orçamento e configurar múltiplos alertas para atearem à medida que se aproxima deste limiar. Os alertas podem ativar um e-mail ou um Grupo de Ação do Azure para efetuar automatização. Nota: a filtragem para esta API não se alinha com a filtragem/dimensões da API de Consulta.
- [API de Orçamentos v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)crie orçamentos com mais capacidades de filtragem de custos do que v1. A filtragem está alinhada com o contrato utilizado nas nossas APIs de Consulta e Dimensões. Esta é a API de orçamentos recomendada para utilizar no futuro.
- [Dimensões:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)fornece operações para obter dimensões suportadas para a sua utilização em vários âmbitos. Ao utilizar a API de Dimensões, pode obter uma lista de dimensões que podem ser utilizadas como entradas para gerar consultas com a API de Consulta.
- [Consulta :](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)fornece operações para obter dados de custo e utilização agregados com base na consulta que fornece. Ao utilizar a API de Consulta, pode especificar a filtragem, ordenação e agrupamento pretendido em todas as dimensões disponíveis (acedidos a partir da API de Dimensões).

**Custos Previstos**

**Por que motivo não vejo previsões para os meus custos na Análise de Custos?**  
Existem vários motivos pelos quais a projeção da previsão pode estar em falta na Análise de Custos e algumas são as seguintes:

1. Se os seus dados de custo têm menos de 10 dias, o gráfico de previsão não será carregado. O modelo requer, pelo menos, 10 dias de dados de custo recentes para projeções precisas
2. Se tiver selecionado datas históricas, o gráfico de previsão não estará visível. Selecione um intervalo de datas com datas futuras para apresentar o gráfico de previsão
3. Se a sua conta tiver múltiplas moedas, o gráfico de previsão apenas irá custar o projeto de "Todos os custos em USD"

**Porque é que a previsão não muda quando faço alterações aos meus recursos?**  
O modelo de previsão necessita de alguns dias para ter em conta as alterações na conta e não efe vezes projeções imediatas com base na alteração de recursos  
Para passos maiores de aumento ou diminuição de recursos, o modelo demorará ligeiramente mais tempo a ajustar-se a estas alterações para ter em conta as dificuldades

**Por que motivo é que a minha previsão aumenta depois de fazer uma reserva ou compra no Marketplace?**  
O modelo de previsão considera o seu "Custo Real" e não contabilia a utilização e a compra em separado. Numa compra única, o modelo irá diminuir as projeções após 10 dias para contabiltar o aumento súbito dos custos

**Quero ver as previsões de uma única dimensão (por exemplo, Metro)**  
Atualmente, a previsão suporta projeções de custos totais e não em metros individuais. Por isso, quando "Agrupado por" uma dimensão, as projeções serão para o total de todos os itens na dimensão

**Documentos recomendados**

- [O que é o Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Práticas recomendadas para Gestão de Custos do Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analisar os seus custos e gastos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorar e analisar custos com a análise de Custos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Preços](https://azure.microsoft.com/services/cost-management/#pricing)
- [Rever custos na análise de custos](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial em vídeo: Criar um orçamento no portal do Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Pré-requisitos para ver e personalizar orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Criar e gerir orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurar automatização com a API de Ações do Azure e Orçamentos](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Utilizar alertas de custos para monitorizar a utilização e os gastos](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Práticas recomendadas de Gestão de Custos](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vídeos de tutorial**

- [Criar um orçamento no portal do Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gerir custos com a API de Orçamentos e os Grupos de Ação](https://go.microsoft.com/fwlink/?linkid=2147038)