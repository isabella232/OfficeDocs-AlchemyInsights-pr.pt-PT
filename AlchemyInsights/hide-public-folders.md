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
# <a name="hide-public-folders"></a><span data-ttu-id="b6c25-102">Ocultar pastas públicas</span><span class="sxs-lookup"><span data-stu-id="b6c25-102">Hide public folders</span></span>

<span data-ttu-id="b6c25-103">**Para esconder toda a árvore da pasta pública:**</span><span class="sxs-lookup"><span data-stu-id="b6c25-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="b6c25-104">Utilize os passos [deste](https://aka.ms/ControlPF) artigo para esconder uma árvore de pasta pública inteira de utilizadores seletivos ou todos os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="b6c25-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="b6c25-105">**Para ocultar uma pasta pública específica:**</span><span class="sxs-lookup"><span data-stu-id="b6c25-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="b6c25-106">Adicionar permissões para utilizadores que precisam de aceder à pasta pública</span><span class="sxs-lookup"><span data-stu-id="b6c25-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="b6c25-107">Remova o **Padrão** do utilizador da lista de **permissões:**</span><span class="sxs-lookup"><span data-stu-id="b6c25-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
