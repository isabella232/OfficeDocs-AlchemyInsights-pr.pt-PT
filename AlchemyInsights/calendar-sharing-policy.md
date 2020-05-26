---
title: 618 Política de Partilha de Calendários
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373010"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erro de política ao partilhar um calendário

1. Faça um dos seguintes, conforme apropriado para a sua situação:
    - Ligue-se ao Exchange Online utilizando a Remote PowerShell. Para mais informações, consulte [Connect to Exchange Online utilizando a Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - No servidor no local, abra a Shell exchange Management.
2. Determine a política de partilha que é atribuída ao utilizador. Para tal, execute o seguinte comando e note a política devolvida:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atualize a política de partilha para o utilizador. To do this, follow these steps:
    - Abra o centro de administração exchange.
    - Clique em **Organização**, e, em seguida, clique duas vezes na política atribuída ao utilizador em **Partilha Individual**. Esta é a política que foi devolvida no passo 2.
    - Na página 'Regra de Partilha', selecione o nível de partilha de calendário que pretende permitir sob **especificar quais as informações que pretende partilhar;** clique **em Guardar**.

Para obter mais informações consulte: ["A política não permite conceder permissões a este nível a um ou mais dos(s)" erro](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)do destinatário quando o utilizador tenta partilhar o calendário .
