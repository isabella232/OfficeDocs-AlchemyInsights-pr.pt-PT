---
title: Criar um e-mail captura tudo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080757"
---
# <a name="create-an-email-catch-all"></a>Criar um e-mail captura tudo

A utilização de um catch all é bastante desconcentrada. É melhor enviar uma mensagem de aviso ao remetente que avisa os remetentes de que a sua mensagem não foi entregue como endereçada para que possam tomar medidas. Também pode limitar a caixa de correio monitorizada para detetar apenas endereços de e-mail anteriormente válidos. 

Qualquer caixa de correio receberá spam em todas as caixas de correio e poderá eventualmente ser preenchida se não for monitorizada de perto. (Existem limites de receção.) 

Se decidir continuar, siga estes passos:

1. Crie um Grupo de Distribuição dinâmico & inclua "Todos os Tipos de Destinatários".

2. Crie uma Caixa de Correio dedicada para capturar e-mails, por exemplo, catchall@domain.com.

3. Para o domínio específico, defina DomainType para "InternalRelay". Se remover a captura de todos, certifique-se de que define o domínio novamente como Autoritativo.

4. Crie uma Regra de Transporte de Fluxo de Correio da seguinte forma:

    - Se o Remetente for "Fora da Organização"
    - Redirecionar a mensagem para o Catchall@domain.com
    - Exceto se o destinatário for membro de um grupo allusers@domain.com (o Grupo de Distribuição contém todos os membros)
    - Certificar-se de que as novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmico
