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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960162"
---
# <a name="problem-with-single-user"></a>Problema com um único utilizador

- O utilizador poderá não ter sido aprovisionado porque o serviço ainda não teve a oportunidade de avaliar o utilizador. Reveja as orientações sobre quanto tempo demora o aprovisionamento, bem como a barra de progresso na página de configuração de aprovisionamento. Se o estado estável especificado na secção detalhes adicionais for anterior à data em que o utilizador foi criado/atualizado/eliminado, significa que ainda não avaliámos o utilizador. Neste cenário, o melhor a fazer é esperar que o serviço de aprovisionamento termine.

  - Tenha em atenção que o nosso serviço só tem conhecimento das alterações feitas a um utilizador no sistema de origem (Cloud HR). Tem de haver uma alteração válida no sistema de origem para o Azure AD para detetar a alteração e a fluir para o Active Directory.
- O serviço de aprovisionamento avaliou o utilizador e determinou que não deveria ser aprovisionado:
  - Se tiver definido um filtro de atribuição com base no prazo, certifique-se de que o utilizador cumpre os critérios que especificou.
  - Se os utilizadores já existirem no sistema de destino e o estado do utilizador na correspondência de origem e destino, não tomaremos nenhuma ação adicional.
- O serviço de aprovisionamento tentou aprovisionar o utilizador e falhou. Para estes cenários, reveja o separador remoção de problemas e recomendações dos registos de aprovisionamento:
  - Um atributo necessário no utilizador pode estar em falta no Active Directory no local ou no Azure AD. Por exemplo, as regras de geração userPrincipalName ou sAMAccountName não estão a gerar o valor certo.
  - O atributo que corresponde (normalmente, IDdeEmpreiteiro) não está a resolver com um utilizador exclusivo no Active Directory no local ou no Azure AD. Por exemplo, existem dois utilizadores com o mesmo ID de funcionário no AD e o serviço devolve um código de erro a indicar entradas de destino duplicadas para a mesma entrada de origem.

Para rever registos de um único utilizador e grupos, consulte Rever os registos de aprovisionamento de [um problema com um utilizador específico.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
