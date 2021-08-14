---
title: Privileged Identity Management função
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973240"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**As permissões não são concedidas após ativar uma função**

Quando ativa uma função no Azure AD Privileged Identity Management (PIM), a ativação pode não propagar instantaneamente todos os portais que exigem a função privilegiada. Por vezes, mesmo que a alteração seja propagada, a cache Web num portal poderá fazer com que a alteração não seja efetuada imediatamente.

Se a ativação estiver atrasada, siga estes passos:

1. Ter saia do portal do Azure e volte a inscrever-se. Quando ativa uma função do Azure AD ou uma função de recurso do Azure, verá as fases da sua ativação. Assim que todas as fases estiverem concluídas, verá uma ligação para "Terminar a suaenização". Pode utilizar esta ligação para sair. Isto irá resolver a maioria dos casos com atrasos de ativação.
2. Em PIM, verifique se está listado como membro da função.
3. Se estiver a ativar a Exchange administrador principal, certifique-se de que sai e volta a inscrever-se. Se o problema persistir, abra um pedido de suporte e levante este problema. Se estiver a utilizar a sua Exchange para aceder ao Centro de Conformidade e Segurança, veja o passo seguinte.
4. Se estiver a ativar uma função para aceder ao Centro de Segurança e Conformidade ou se estiver a ativar a função de Administrador do SharePoint, irá detetar algum atraso de ativação de alguns minutos até algumas horas. Este é um problema conhecido e estamos a trabalhar ativamente com estas equipas para resolver este problema o mais rapidamente possível.

Para mais informações, consulte:

- [Ativar as minhas funções do Azure AD no PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Ativar as minhas funções de recurso do Azure no PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**As permissões não são removidas após desativar uma função ou a função de ativação expirar**

Quando desativa uma função no Azure AD Privileged Identity Management ou quando expira um período de ativação da função, poderá haver um atraso no qual continua a ter acesso.

Se a sua desativação estiver atrasada, siga estes passos:

1. Se estiver a desativar a função de Administrador do Exchange ou a função período de ativação expirar e notar um atraso significativo antes de as permissões serem removidas, abra um pedido de suporte e informe o seu engenheiro de suporte para o ajudar a arquivar um pedido na equipa de Gestão de Acesso Privilegiado (PAM) do Office sobre este problema.
2. Se o período de ativação tiver expirado, mas ainda tiver a sessão do browser aberta, feche o browser. Pode continuar a utilizar a função até fechar essa sessão. Este é um problema conhecido e estamos a procurar uma possível correção para revogar ativamente cada sessão após a ativação expirar.

Se o seu atraso for diferente destes dois cenários, abra um bilhete de suporte.
