---
title: Ocultar pastas públicas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315436"
---
# <a name="hide-public-folders"></a>Ocultar pastas públicas

**Para esconder toda a árvore da pasta pública:**

Utilize os passos [deste](https://aka.ms/ControlPF) artigo para esconder uma árvore de pasta pública inteira de utilizadores seletivos ou todos os utilizadores.

**Para ocultar uma pasta pública específica:**

1. Adicionar permissões para utilizadores que precisam de aceder à pasta pública

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Remova o **Padrão** do utilizador da lista de **permissões:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
