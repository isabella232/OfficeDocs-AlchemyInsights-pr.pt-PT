---
title: Configurar o serviço de Aprovisionamento
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033289"
---
# <a name="configuring-the-provision-service"></a>Configurar o serviço de Aprovisionamento

Para que o aprovisionamento automático de utilizadores funcione, o Azure AD requer credenciais válidas que lhe permitam ligar à API dos Serviços Web Workday. Além disso, o botão Testar Ligação na aplicação Workday to AD User Provisioning também valida se conseguir ligar ao Azure AD Ligação provisioning Agent associado ao Domínio AD.

Se o portal do Azure devolver um erro ao guardar as credenciais, siga os passos recomendados abaixo:

1. Confirme que configurou a conta de Utilizador do Utilizador do Sistema de Integração de Dia de Trabalho conforme apresentado na secção tutorial Configurar o utilizador do sistema de integração [no Dia de Trabalho.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Confirme que o Serviço do Azure AD Ligação Agente de Aprovisionamento está a funcionar no seu servidor de Windows no local através da Consola de Gestão de Serviços. Também pode verificar o estado do agente no portal do Azure ao clicar no botão Ver agentes no local.
3. Certifique-se de que está a introduzir o valor do campo "Nome de Utilizador do Dia de Trabalho" utilizando o formato username@workday-nome-de-inquilino. Se o nome do inquilino-dia de trabalho estiver em falta, a autenticação dia de trabalho falha.
4. Se estiver a configurar a integração com o inquilino de implementação Dia de Trabalho, tenha em atenção as horas de inatividade agendadas do seu inquilino Dia de Trabalho. O dia de trabalho tem um tempo de desatualização agendado para os inquilinos de implementação ao longo dos fins de semana (normalmente da sexta-feira à noite até sábado de manhã) e as falhas de conectividade durante esta janela de tempo de inatividade são um problema conhecido que resolve automaticamente assim que os inquilinos de implementação ficarem novamente online.
5. Em casos raros, também poderá ver este erro se a palavra-passe do Utilizador do Sistema de Integração tiver sido alterada devido à atualização do inquilino ou se a conta estiver bloqueada ou tiver expirado. Verifique o estado do utilizador do Sistema de Integração com o seu administrador de Dia de Trabalho.

Para obter mais detalhes sobre como configurar o dia de trabalho para o aprovisionamento automatizado, consulte [Tutorial: Configurar](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)Dia de Trabalho para o aprovisionamento automático de utilizadores.
