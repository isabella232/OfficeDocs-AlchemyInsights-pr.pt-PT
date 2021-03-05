---
title: Provisão de utilizadores
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481883"
---
# <a name="user-provisioning"></a>Provisão de utilizadores

- Utilize a capacidade [de provisionamento a pedido](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) para provisionar um utilizador e obter diagnósticos detalhados sobre as medidas tomadas.
- Para resolver problemas que encontra ao providenciar utilizadores e grupos, consulte o guia de resolução de problemas [Que não estão a ser abastetados](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Se observar que os utilizadores não estão a ser a provisionados, consulte [os registos de provisionamento (pré-visualização)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) no Diretório Ativo Azure (AD). Procure por entradas de registo relativas a um utilizador específico.
- Reinicie periodicamente o provisionamento para capturar os utilizadores que não tenham sido recívais num ciclo de provisionamento anterior.
- O utilizador/grupo pode não ter sido a provisionado porque o nosso serviço ainda não teve oportunidade de avaliar o utilizador. Reveja as orientações para o tempo de provisão, bem como a barra de progresso na página de configuração de provisionamento. Se o estado estacionário especificado na secção de detalhes adicionais for antes da data em que o utilizador foi criado/atualizado/eliminado, significa que ainda não avaliámos o utilizador. Neste cenário, a melhor coisa a fazer é esperar que o serviço de prestação termine. Se o estado estável tiver sido alcançado, recomendamos a realização de um reinício da UI no Portal Azure.
  - Note que o nosso serviço só tem conhecimento de alterações a um utilizador/grupo no sistema de origem (Azure Ative Directory). Se um utilizador/grupo for removido diretamente na aplicação (por exemplo, ServiceNow), não temos conhecimento dessas alterações e não a revogamos com base no estado do utilizador no sistema de origem. Neste cenário, o melhor é reverter a mudança diretamente na aplicação-alvo.
- O nosso serviço avaliou o utilizador/grupo e determinou que não deveria ser a provisionado:
  - Se definiu o âmbito para utilizadores e grupos designados, verifique se o utilizador/grupo está atribuído à aplicação.
  - Se o utilizador/grupo for atribuído à aplicação, certifique-se de que não estão atribuídos à função de acesso predefinido. Esta função não pode ser utilizada para o provisionamento.
  - Se tiver definido um filtro de deteção baseado em atributos, certifique-se de que o utilizador satisfaz os critérios especificados.
  - Se os utilizadores já existirem no sistema-alvo e no estado do utilizador na origem e no target match, não tomaremos mais nenhuma ação.
- O nosso serviço tentou abastecer o utilizador e falhou. Para estes cenários, reveja o separador de resolução de problemas e recomendações dos registos de provisionamento:
  - Um atributo necessário para o utilizador pode estar em falta no Diretório Azure Ative ou não corresponde ao formato exigido pela aplicação de terceiros. Por exemplo, o atributo País num utilizador pode ser definido para os Estados Unidos quando deveria ser EUA.
  - O atributo é um atributo referencial que ainda não existe na aplicação-alvo. Um atributo referencial é um atributo que aponta para outro objeto, por exemplo, um utilizador que é membro de um grupo. O ID do utilizador estaria no atributo de membro do grupo, mas só pode ser processado se o objeto do utilizador o contestar já existir.
