---
title: Aprovisionamento de utilizadores
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971350"
---
# <a name="user-provisioning"></a>Aprovisionamento de utilizadores

- Utilize a [capacidade de aprovisionamento](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) a pedido para aprovisionar um utilizador e obter diagnósticos detalhados sobre os passos dados.
- Para refletir problemas que encontra ao aprovisionar utilizadores e grupos, consulte o guia de remoção de problemas Nenhum utilizador está [a ser aprovisionado.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Se observar que os utilizadores não estão a ser aprovisionados, consulte o artigo Aprovisionar registos [(pré-visualização)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) em Azure Active Directory (AD). Procure entradas de registo específicas de um utilizador específico.
- Reinicie periodicamente o aprovisionamento para detetar quaisquer utilizadores perdidos num ciclo de aprovisionamento anterior.
- O utilizador/grupo poderá não ter sido aprovisionado porque o nosso serviço ainda não teve a oportunidade de avaliar o utilizador. Reveja as orientações sobre quanto tempo demora o aprovisionamento, bem como a barra de progresso na página de configuração de aprovisionamento. Se o estado estável especificado na secção detalhes adicionais for anterior à data em que o utilizador foi criado/atualizado/eliminado, significa que ainda não avaliámos o utilizador. Neste cenário, o melhor a fazer é esperar que o serviço de aprovisionamento termine. Se o estado estável tiver sido alcançado, recomendamos que execute um reinício da IU no Portal do Azure.
  - Tenha em atenção que o nosso serviço só tem conhecimento das alterações feitas a um utilizador/grupo no sistema de origem (Azure Active Directory). Se um utilizador/grupo for removido diretamente na aplicação (por exemplo, ServiceNow), não temos conhecimento dessas alterações e não as recuaremos com base no estado do utilizador no sistema de origem. Neste cenário, é melhor recuar a alteração diretamente na aplicação de destino.
- O nosso serviço avaliou o utilizador/grupo e determinou que não deveria ser aprovisionado:
  - Se tiver definido o âmbito para utilizadores e grupos atribuídos, verifique se o utilizador/grupo está atribuído à aplicação.
  - Se o utilizador/grupo estiver atribuído à aplicação, certifique-se de que não está atribuída à função de acesso predefinida. Esta função não pode ser utilizada para aprovisionamento.
  - Se tiver definido um filtro de atribuição com base no prazo, certifique-se de que o utilizador cumpre os critérios que especificou.
  - Se os utilizadores já existirem no sistema de destino e o estado do utilizador na correspondência de origem e destino, não tomaremos nenhuma ação adicional.
- O nosso serviço tentou aprovisionar o utilizador e falhou. Para estes cenários, reveja o separador remoção de problemas e recomendações dos registos de aprovisionamento:
  - Um atributo necessário no utilizador pode estar em falta no Azure Active Directory ou não corresponder ao formato exigido pela aplicação de terceiros. Por exemplo, o atributo País num utilizador pode estar definido para Estados Unidos da América quando deveria ser dos EUA.
  - O atributo é um atributo referencial que ainda não existe na aplicação de destino. Um atributo referencial é um atributo que aponta para outro objeto, por exemplo, um utilizador que seja membro de um grupo. O ID do utilizador estaria no atributo de membro do grupo, mas só pode ser processado se o objeto de utilizador apontar para já existir.
