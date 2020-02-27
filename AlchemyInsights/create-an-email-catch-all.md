---
title: Criar um e-mail catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286203"
---
# <a name="create-an-email-catch-all"></a>Criar um e-mail catch all

A utilização de uma captura é fortemente desencorajada. É melhor dar um salto de volta ao remetente, deixando os remetentes saberem que a sua mensagem não poderia ser entregue como endereçada para que possam tomar medidas. Também pode limitar a caixa de correio monitorizada apenas para capturar endereços de e-mail anteriormente válidos. 

Qualquer captura, todas as caixas de correio receberão uma boa dose de spam e poderão eventualmente preencher se não forem monitorizadas de perto. (Há limites de receção.) 

Se decidir prosseguir, siga estes passos:

1. Criar um Grupo de Distribuição Dinâmica & incluir "Todos os tipos de destinatários".

2. Crie uma Caixa de Correio dedicada para apanhar e-mails, por exemplo, catchall@domain.com.

3. Para o domínio específico, desloque o DomainType para "InternalRelay". Se remover mais tarde a captura, certifique-se de que o domínio volta a ser Autorizado.

4. Crie uma Regra de Transporte de Fluxos de Correio da seguinte forma:

    - Se o Remetente estiver "Fora da Organização"
    - Redirecione a mensagem para Catchall@domain.com
    - Exceto se o destinatário for membro da allusers@domain.com (Grupo de Distribuição contém todos os membros)
    - Certifique-se de validar que novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmica
