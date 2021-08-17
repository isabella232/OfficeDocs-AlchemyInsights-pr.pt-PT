---
title: 618 - Política de Partilha de Calendários
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091614"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erro de política ao partilhar um calendário

1. Eis um dos seguintes procedimentos, conforme adequado à sua situação:
    - Ligação a Exchange Online através do PowerShell Remoto. Para obter mais informações, [consulte Ligação utilizar Exchange Online PowerShell Remoto.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - No servidor no local, abra a Shell de Gestão Exchange dados.
2. Determine a política de partilha atribuída ao utilizador. Para tal, execute o seguinte comando e anote a política devolvida:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atualize a política de partilha do utilizador. Para tal, siga estes passos:
    - Abra o Exchange de administração.
    - Clique **em Organização** e, em seguida, faça duplo clique na política atribuída ao utilizador em Partilha **Individual.** Esta é a política devolvida no passo 2.
    - Na página Regra de Partilha, selecione o nível de partilha de calendário que pretende permitir em **Especifique as informações que pretende partilhar;** clique **em Guardar**.

Para obter mais informações, consulte: Erro "A política não permite a concessão de permissões a este nível para um ou mais dos [destinatários",](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)quando o utilizador tenta partilhar o calendário .
