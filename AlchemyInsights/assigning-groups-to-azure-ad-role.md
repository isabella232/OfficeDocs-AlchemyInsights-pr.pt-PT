---
title: Atribuir grupos para o papel de AD Azure
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885394"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Atribuir grupos para o papel de AD Azure

Para atribuir um grupo AD Azure com fonte de autoridade em Azure AD a um papel de AD Azure, execute os seguintes passos:

1. Criar um novo grupo - Criar um novo grupo:

    a. Inscreva-se no centro de administração Azure AD com **funções privilegiadas de administrador** ou permissões **globais de administrador.**
    b. Selecione **Azure Ative Directory > Groups > Todos os grupos > Novo grupo**.
    c. Criar o grupo.

2. Atribua o papel ao grupo durante a criação do grupo ou após a criação do grupo.

    a. Para atribuir um papel ao grupo no momento da criação do grupo, ligue as **funções de AD Azure** pode ser atribuída ao grupo e criar o grupo.
    b. Para atribuir um papel ao grupo depois de criado, navegue no separador **de funções atribuído** para o grupo recém-criado e atribua o papel ao grupo.  

**Gerir a adesão a um grupo que é atribuído ao papel de Azure AD**

Para evitar a elevação de privilégios, por defeito, apenas administradores privilegiados e administradores globais podem modificar a adesão de um grupo que é atribuído a um papel. Podem, no entanto, optar por designar um proprietário para tal grupo e delegar esta tarefa.

Para obter mais detalhes sobre a atribuição de grupos de nuvem a funções AD Azure, consulte [atribuir uma função de AD ao Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Para obter mais detalhes sobre as funções de resolução de problemas atribuídos a grupos de nuvem, consulte [as funções de resolução de problemas atribuídas a grupos de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





