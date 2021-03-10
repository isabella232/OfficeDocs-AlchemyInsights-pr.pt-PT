---
title: Corrigir a política do arrendatário (sobreposição de ação)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695697"
---
# <a name="fix-tenant-policy-action-override"></a>Corrigir a política do arrendatário (sobreposição de ação)

Uma política anti-correio publicitário não-correio eletrónico no seu inquilino afetou esta mensagem. Para rever a política, faça o seguinte:

1. Vá ao [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), e depois vá para a Política de **Gestão** de Ameaças  >    >  [Antisspam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Verifique se a **fonte de política** indica o seguinte:  **Add-Xheader/ModificarSubject/Redirect/Delete/No action/ BCC message**

    Em caso afirmativo, no separador **'Personalizado',** verifique as definições da política que afetou a mensagem. É possível que as **definições Standard aplicadas** a todos os clientes da Exchange Online Protection afetassem a mensagem.

Para obter mais informações sobre as políticas de filtragem de spam, consulte [configurar as suas políticas de filtro de spam](https://go.microsoft.com/fwlink/?linkid=2101431).
