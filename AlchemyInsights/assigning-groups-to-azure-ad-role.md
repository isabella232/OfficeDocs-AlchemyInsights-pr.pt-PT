---
title: Atribuir grupos à função Azure AD
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
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036251"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Atribuir grupos à função Azure AD

Para atribuir uma função do Azure AD ao grupo de origem da autoridade no Azure AD, efetue os seguintes passos:

1. Criar um novo grupo - Para criar um novo grupo:

    a. Inscreva-se no centro de administração do Azure AD com permissões **de administrador** privilegiado de funções ou de **administrador global.**
    b. **Selecione Azure Active Directory > Grupos > Todos os > Grupo Novo.**
    c. Crie o grupo.

2. Atribuir a função ao grupo durante a criação do grupo ou após a criação do mesmo.

    a. Para atribuir uma função ao grupo na altura da criação de grupos, ativo o botão de alternar Funções do **Azure AD** pode ser atribuído ao grupo e criar o mesmo.
    b. Para atribuir uma função ao grupo após ter sido criado, navegue para o separador Funções **atribuídas** para o grupo criado recém-criado e atribuir a função ao grupo.  

**Gerir a associação de um grupo atribuído à função Azure AD**

Para impedir a elevação de privilégios, por predefinição, apenas os administradores de funções privilegiados e os administradores globais podem modificar a associação de um grupo a que está atribuída uma função. No entanto, podem optar por atribuir um proprietário a esse grupo e delegar esta tarefa.

Para obter mais detalhes sobre como atribuir grupos na nuvem a funções do Azure AD, consulte Atribuir funções de AD ao Grupo na [Nuvem.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Para obter mais detalhes sobre as funções de remoção de problemas atribuídas a grupos na nuvem, consulte Remoção de funções atribuídas a grupos na [nuvem.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





