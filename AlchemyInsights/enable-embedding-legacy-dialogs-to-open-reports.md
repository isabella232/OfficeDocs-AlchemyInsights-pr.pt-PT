---
title: Ativar caixas de diálogo incorporadas para abrir relatórios
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814275"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Ativar caixas de diálogo incorporadas para abrir relatórios

**Sintoma**

Os utilizadores não conseguem abrir relatórios. "Algo correu mal. Consulte detalhes técnicos para obter mais detalhes. "

**Causa**

Os relatórios não estão a carregar o UCI com o erro, "o descritor de formulários é nulo ou não está definido". Os relatórios no UCI ainda requerem caixas de diálogo legadas, por isso, o sistema do cliente precisa de ter *allowlegacydialogsembedding* ativadadas.

**Solução**

1. Aceda a **Definições > Administração > Definições do sistema > Separador Geral**.

2. Defina "Ativar a incorporação de determinadas caixas de diálogo legadas no cliente do browser da interface unificada" para **Sim**.
