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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003400"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Ativar caixas de diálogo incorporadas para abrir relatórios

**Sintoma**

Os utilizadores não conseguem abrir relatórios. "Algo correu mal. Consulte os detalhes técnicos para obter mais detalhes. "

**Causa**

Os relatórios não estão a carregar o UCI com o erro "o descritor de formulários é nulo ou não está definido". Os relatórios no UCI ainda requerem caixas de diálogo legadas, por isso, o sistema do cliente precisa de ter *allowlegacydialogsembedding* ativadas.

**Solução**

1. Aceda a **Definições > Administração > Definições do sistema > Separador Geral**.

2. Defina "Ativar a incorporação de determinadas caixas de diálogo legadas no cliente do browser da interface unificada" para **Sim**.
