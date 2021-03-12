---
title: Conjunto de réplica
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714254"
---
# <a name="replica-set"></a>Conjunto de réplica

O AADDS também é chamado como o domínio gerido. Na verdade, são dois controladores de domínio que são executados e mantidos pelo backend. Os dois DCs incluem um DC principal e um DC de replicação. As cópias de segurança em AADDS (domínio gerido) são um processo automatizado gerido pela plataforma Azure. Em caso de problema com o seu domínio gerido, o suporte Azure pode ajudá-lo a restaurar a partir de backup.

Cria-se cada conjunto de réplicas numa rede virtual. Cada rede virtual deve ser espreitada para todas as outras redes virtuais que hospedam um conjunto de réplicas de domínio gerido. Esta configuração cria uma topologia de rede de malha que suporta a replicação do diretório. Uma rede virtual pode suportar vários conjuntos de réplicas, desde que cada conjunto de réplicas esteja numa sub-rede virtual diferente.

Para obter mais detalhes sobre o conjunto de [réplicas, consulte os conjuntos de réplicas de conceitos.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
