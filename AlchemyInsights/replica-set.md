---
title: Conjunto de réplicas
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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110691"
---
# <a name="replica-set"></a>Conjunto de réplicas

O AADDS também é denominado domínio gerido. Na verdade, são dois controladores de domínio que são executados e mantidos pelo back-end. Os dois DCs incluem um DC principal e um DC de replicação. As cópias de segurança no AADDS (domínio gerido) são um processo automatizado gerido pela plataforma do Azure. Em caso de problema com o seu domínio gerido, o suporte do Azure pode ajudá-lo no restauro da cópia de segurança.

Pode criar cada conjunto de réplicas numa rede virtual. Cada rede virtual tem de ser peered para todas as outras redes virtuais que alojam o conjunto de réplicas de um domínio gerido. Esta configuração cria uma topologia de rede de malha que suporta a replicação de diretórios. Uma rede virtual pode suportar múltiplos conjuntos de réplicas, desde que cada conjunto de réplicas esteja numa sub-rede virtual diferente.

Para obter mais detalhes sobre o conjunto de Replicação, consulte [Conjuntos de Replicação de Conceitos.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
