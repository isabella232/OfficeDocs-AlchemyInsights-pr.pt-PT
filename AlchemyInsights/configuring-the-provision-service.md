---
title: Configuração do serviço de Provisão
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484050"
---
# <a name="configuring-the-provision-service"></a>Configuração do serviço de Provisão

Para o fornecimento automatizado de utilizadores para funcionar, o Azure AD requer credenciais válidas que lhe permitem ligar-se à API dos Serviços Web workday. Além disso, o botão de Ligação de Teste no Dia de Trabalho para a aplicação de provisionamento do utilizador AD também valida se for capaz de se ligar ao Agente de Provisionamento AD AD Ad associado ao Domínio AD.

Se o portal Azure estiver a devolver um erro ao guardar as credenciais, siga os passos recomendados abaixo:

1. Confirme que configura a conta do Utilizador do Sistema de Integração workday, conforme indicado na secção tutorial [Configure o utilizador do sistema de integração no Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Confirme que o Serviço de Agente de Provisionamento AD AD AZure está a funcionar no seu servidor Windows no local utilizando a Consola de Gestão de Serviços. Também pode verificar o estado do agente no portal Azure clicando no botão Ver agentes no local.
3. Certifique-se de que está a introduzir o valor para o campo "Nome de Utilizador workday" utilizando o formato username@workday-nome de inquilino. Se faltar o nome do inquilino do dia de trabalho, a autenticação do workday falha.
4. Se estiver a configurar a integração com o inquilino de implementação workday, observe as horas de inatividade programadas do seu inquilino workday. O workday tem programado tempo de inatividade para os seus inquilinos de implementação durante os fins de semana (geralmente de sexta-feira à noite para sábado de manhã) e falhas de conectividade durante esta janela de tempo de inatividade é uma questão conhecida que resolve automaticamente assim que os inquilinos de implementação estão novamente on-line.
5. Em casos raros, poderá também ver este erro se a palavra-passe do Utilizador do Sistema de Integração for alterada devido à atualização do arrendatário ou se a conta estiver em estado fechado ou caducado. Verifique o estado do utilizador do Sistema de Integração com o seu administrador workday.

Para obter mais informações sobre a configuração do dia de trabalho para o provisionamento automatizado, consulte [Tutorial: Configure Workday para o provisionamento automático do utilizador](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
