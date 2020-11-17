---
title: Papel privilegiado de Gestão de Identidade
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088876"
---
# <a name="privileged-identity-managementpim-role"></a>Papel privilegiado de Gestão de Identidade (PIM)

**As permissões não são concedidas após a ativação de uma função**

Quando ativar uma função na Gestão de Identidade Privilegiada AD Azure (PIM), a ativação pode não se propagar instantaneamente a todos os portais que requerem o papel privilegiado. Por vezes, mesmo que a mudança seja propagada, o caching web num portal pode resultar na alteração não ter efeito imediatamente.

Se a sua ativação for retardada, siga estes passos:

1. Assine fora do portal Azure e depois volte a entrar. Quando ativar uma função AD Azure ou uma função de recurso Azure, verá as fases da sua ativação. Uma vez concluídas todas as etapas, verá um link 'Sign out'. Pode usar este link para assinar. Isto resolverá a maioria dos casos para atraso de ativação.
2. Na PIM, verifique se está listado como membro do papel.
3. Se estiver a ativar a função de Administrador de Troca, certifique-se de que assina e volta a entrar. Se o problema persistir, abra um bilhete de apoio e levante-o como um problema. Se estiver a utilizar a sua função de Administrador de Intercâmbio para aceder ao Centro de Segurança e Conformidade, consulte o próximo passo.
4. Se estiver a ativar uma função para aceder ao Centro de Segurança e Conformidade ou se estiver a ativar a função de Administrador SharePoint, sentirá algum atraso de ativação de alguns minutos até algumas horas. Esta é uma questão conhecida e estamos a trabalhar ativamente com estas equipas para resolver esta questão o mais rapidamente possível.

Para obter mais informações, consulte:

- [Ativar os meus papéis de AD Azure em PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Ativar os meus papéis de recurso Azure na PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**As permissões não são removidas após desativar uma função ou a ativação da função expira**

Quando desativa um papel na Gestão de Identidade Privilegiada AD Azure ou quando um período de ativação de funções expirar, pode haver um atraso onde continua a ter acesso.

Se a sua desativação for adiada, siga estes passos:

1. Se estiver a desativar a função de Administrador de Câmbio ou o período de ativação da função expirar, e notar um atraso significativo antes de as permissões serem removidas, abra um bilhete de apoio e diga ao seu engenheiro de suporte para o ajudar a arquivar um bilhete com a equipa de Gestão de Acesso Privilegiado (PAM) dentro do Office sobre este assunto.
2. Se o período de ativação tiver expirado, mas ainda tiver a sessão do navegador aberta, feche o seu navegador. Pode continuar a usar o papel até encerrar a sessão. Esta é uma questão conhecida e estamos a estudar uma possível correção para revogar ativamente cada sessão uma vez expirada a ativação.

Se o seu atraso for diferente destes dois cenários, por favor abra um bilhete de apoio.
