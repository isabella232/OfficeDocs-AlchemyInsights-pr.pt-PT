---
title: Problema com um único utilizador
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430203"
---
# <a name="problem-with-single-user"></a>Problema com um único utilizador

- O utilizador pode não ter sido prestado porque o serviço ainda não teve oportunidade de avaliar o utilizador. Reveja as orientações para o tempo de provisão, bem como a barra de progresso na página de configuração de provisionamento. Se o estado estacionário especificado na secção de detalhes adicionais for antes da data em que o utilizador foi criado/atualizado/eliminado, significa que ainda não avaliámos o utilizador. Neste cenário, a melhor coisa a fazer é esperar que o serviço de prestação termine.

  - Note que o nosso serviço só tem conhecimento de alterações a um utilizador no sistema de origem (Cloud HR). Tem de haver uma alteração válida no sistema de origem para a Azure AD detetar a mudança e fluí-la para o Ative Directory.
- O serviço de prestação avaliou o utilizador e determinou que não deveria ser a provisionado:
  - Se tiver definido um filtro de deteção baseado em atributos, certifique-se de que o utilizador satisfaz os critérios especificados.
  - Se os utilizadores já existirem no sistema-alvo e no estado do utilizador na origem e no target match, não tomaremos mais nenhuma ação.
- O serviço de fornecimento tentou forrar o utilizador e falhou. Para estes cenários, reveja o separador de resolução de problemas e recomendações dos registos de provisionamento:
  - Um atributo necessário para o utilizador pode estar em falta no Ative Directory ou Azure AD. Por exemplo, as regras de geração do userPrincipalName ou sAMAccountName não estão a gerar o valor certo.
  - O atributo correspondente (geralmente employeeId) não está a ser resolvida para um utilizador único no Ative Directory ou AZure AD. Por exemplo, existem dois utilizadores com o mesmo colaboradorId em AD e o serviço devolve um código de erro indica entradas-alvo duplicadas para a mesma entrada de origem.

Para rever os registos de um único utilizador e grupos, consulte [rever os registos de provisionamento para um problema com um utilizador específico](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
