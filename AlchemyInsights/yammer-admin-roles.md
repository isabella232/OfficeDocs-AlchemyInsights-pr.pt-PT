---
title: Sobre os administradores de Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038121"
---
# <a name="about-yammer-admins"></a>Sobre os administradores de Yammer

**Administradores de rede**

Os administradores globais são automaticamente promovidos ao papel de Administrador Verificado numa rede Yammer. Nos seguintes casos, esta promoção pode não ocorrer corretamente:

- Existem várias redes Yammer, e o administrador está a ser assinado na errada. [A consolidação da rede](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) é necessária para chegar a uma rede Yammer.
- O Azure PIM está a ser usado. O utilizador não pode ser promovido a administrador global tempo suficiente para que a promoção ocorra. Uma futura atualização para a Yammer pode resolver este problema, mas o melhor é promover os utilizadores para administração global manualmente.
- Existe um problema de sincronização com a rede Yammer. Neste caso, será necessário um pedido de apoio para uma investigação mais aprofundada.

Para obter mais informações sobre os papéis de administrador da Yammer, consulte [administração Manage Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Administradores de grupo**

Os administradores do grupo para grupos conectados microsoft 365 estão sincronizados com a adesão do grupo a Azure AD. Para os grandes grupos, esta sincronização pode demorar um período prolongado.
