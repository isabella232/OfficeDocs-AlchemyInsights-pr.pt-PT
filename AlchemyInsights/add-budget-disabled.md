---
title: Porque é que o botão de orçamento add está desativado para mim?
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
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822646"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Porque é que o botão de orçamento add está desativado para mim?

Para criar um orçamento, precisa de uma das seguintes permissões:

- Grupo de Gestão, Subscrição, Âmbitos do Grupo de Recursos
- Contribuidor para a Gestão de Custos
- Proprietário
- Contribuinte
- Apenas cliente empresarial: Inscrição, Departamento, Âmbitos de Conta
- Administrador de Inscrição (orçamento definido no âmbito de inscrição)
- Administração do Departamento (orçamento definido no âmbito do Departamento)
- Proprietário de Conta (orçamento definido no âmbito da conta)
- Apenas contrato de cliente moderno: conta de faturação, perfil de faturação, âmbitos de secção de fatura
- Criador de subscrição Azure

**Criei um orçamento quando o meu custo para o mês em curso já estava sobre-orçamentado. Por que não recebi um alerta?**  
Se já excedeu um determinado limiar de custos quando criar um orçamento esse alerta não disparará. Uma vez que um novo ciclo começa, se quebrar o limiar, então o alerta disparará.

**Quando devo esperar receber um alerta depois de exceder um dos meus limiares de alerta orçamental definidos?**  
Os orçamentos são avaliados a cada 4 horas. Leva um mínimo de 8 horas para os dados de utilização chegarem ao sistema orçamental. Perante isto, os alertas podem demorar até 12 horas a disparar depois de exceder um limiar.

**Porque é que o botão de data de início é desativado quando seleciono um período de reset mensal de um mês de mês de mês de faturação?**  
Os orçamentos estão alinhados com o mês civil em vigor ou o período de faturação atual (no caso de ser selecionado o Mês de Faturação). Portanto, preenchamos este valor para si.

**Por que não vejo um gráfico dos meus custos na experiência de criação de orçamento?**  
Precisamos de um mínimo de 2 meses de dados de custos antes de podermos fazer um gráfico para ajudá-lo na criação de orçamento.

**Por que não posso definir um orçamento contra uma assinatura que acabei de criar?**  
Após a criação de uma subscrição, os dados demoram 24-48 horas a processar antes de definir um orçamento contra ele.

**Recursos da API orçamental**

- [Orçamentos API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Disponibiliza operações para criar e atualizar orçamentos. Utilizando a API dos Orçamentos, pode definir um limiar orçamental e configurar vários alertas para disparar à medida que se aproxima desse limiar. Os alertas podem desencadear um e-mail ou um Grupo de Ação Azure para realizar automatização. Nota: A filtragem para esta API não se alinha com a filtragem/dimensões da API de consulta.
- [Orçamentos API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Criar orçamentos com maior capacidade de filtragem de custos do que v1. A filtragem alinha-se com o contrato utilizado nas nossas APIs de Consulta e Dimensões. Estes são os orçamentos recomendados que a API deve utilizar para avançar.
- [Dimensões](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Fornece operações para obter dimensões suportadas para a sua utilização sob uma variedade de âmbitos. Utilizando a API dimensionais, pode obter uma lista de dimensões que podem ser usadas como entradas para gerar consultas com a API de Consulta.
- [Consulta](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Fornece operações para obter dados de custos e utilização agregados com base na consulta que fornece. Utilizando a API de consulta, pode especificar a filtragem, triagem e agrupamento desejados em todas as dimensões disponíveis (que são acedidas a partir da API dimensional).

**Custos Previstos**

**Por que não vejo previsões para os meus custos na Análise de Custos?**  
Existem várias razões pelas quais a projeção da previsão pode estar faltando para si na Análise de Custos, algumas delas são as seguintes:

1. Se os seus dados de custos tão velhos com menos de 10 dias, o gráfico de previsão não será carregado. O modelo requer pelo menos 10 dias de dados de custos recentes para projeções precisas
2. Se tiver selecionado datas históricas, o gráfico de previsão não será visível. Por favor, selecione um intervalo de datas com datas futuras para o gráfico de previsão a ser exibido
3. Se a sua conta tiver várias moedas, o gráfico de previsão só irá projetar os custos de "Todos os custos em USD"

**Porque é que a previsão não muda quando faço alterações nos meus recursos?**  
O modelo de previsão requer alguns dias para ter em conta as alterações na conta e não faz projeções imediatas com base na mudança de recursos  
Para maiores passos de aumento ou diminuição de recursos, o modelo demorará um pouco mais tempo a ajustar-se a estas alterações para ter em conta as anomalias

**Porque é que a minha previsão aumenta depois de fazer uma reserva ou comprar o Marketplace?**  
O modelo de previsão considera o seu "Custo Real" e não explica a utilização e a compra separadamente. Para uma compra única, o modelo diminuirá as projeções após 10 dias para explicar o súbito aumento dos custos

**Quero ver previsões para uma única dimensão (por exemplo. Contador)**  
A previsão suporta atualmente projeções totais de custos e não para contadores individuais. Assim, quando 'Agrupados por' uma dimensão, as projeções serão para o total de todos os itens na dimensão

**Documentos Recomendados**

- [O que é Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management boas práticas](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analise os seus custos e gastos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explore e analise os custos com a análise de custos](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Preços](https://azure.microsoft.com/services/cost-management/#pricing)
- [Rever os custos na análise de custos](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Vídeo tutorial: Criar um orçamento no portal Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Pré-requisitos para visualização e personalização de orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Criar e gerir orçamentos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configure a automação com grupos de ação Azure e Orçamentos API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Use alertas de custos para monitorizar o uso e gastos](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gestão de Custos das melhores práticas](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vídeos tutoriais**

- [Criar um orçamento no portal Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gerir custos com a API dos Orçamentos e grupos de ação](https://go.microsoft.com/fwlink/?linkid=2147038)