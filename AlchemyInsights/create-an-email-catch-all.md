---
title: Criar um e-mail catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712997"
---
# <a name="create-an-email-catch-all"></a>Criar um e-mail catch all

A utilização de uma captura é fortemente desencorajada. É melhor dar um salto de volta ao remetente, informando os remetentes que a sua mensagem não possa ser entregue como endereçado, para que possam tomar medidas. Também pode limitar a caixa de correio monitorizada apenas para capturar endereços de e-mail anteriormente válidos. 

Qualquer captura de toda a caixa de correio receberá uma boa dose de spam e poderá eventualmente preencher se não for monitorizada de perto. (Existem limites de receção.) 

Se decidir prosseguir, siga estes passos:

1. Criar um grupo de distribuição dinâmica & inclua "Todos os tipos de destinatários".

2. Crie uma caixa de correio dedicada para apanhar e-mails, por exemplo, catchall@domain.com.

3. Para o domínio específico, desaprote o 'DomainType' para "InternalRelay". Se mais tarde retirar todas as capturas, certifique-se de que devolve o domínio ao Autoritário.

4. Criar uma Regra de Transporte de Fluxo de Correio da seguinte forma:

    - Se o Remetente estiver "Fora da Organização"
    - Redirecione a mensagem para Catchall@domain.com
    - Exceto se o destinatário for membro da allusers@domain.com (o Grupo de Distribuição contém todos os membros)
    - Certifique-se de validar que novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmica
