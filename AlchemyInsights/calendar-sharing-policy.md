---
title: 618 Política de Partilha de Calendários
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684241"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Erro de política ao partilhar um calendário

1. Faça uma das seguintes, conforme apropriado para a sua situação:
    - Conecte-se a Exchange Online utilizando o Remote PowerShell. Para obter mais informações, consulte [Connect to Exchange Online utilizando Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - No servidor no local, abra a Shell de Gestão de Câmbios.
2. Determine a política de partilha que é atribuída ao utilizador. Para isso, executar o seguinte comando e observar a apólice devolvida:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Atualize a política de partilha para o utilizador. Para tal, siga estes passos:
    - Abra o centro de administração Exchange.
    - Clique em **Organização**e, em seguida, clique duas vezes na política que é atribuída ao utilizador em **Partilha Individual**. Esta é a política que foi devolvida no passo 2.
    - Na página 'Regra de Partilha', selecione o nível de partilha de calendário que pretende permitir em **Especificar as informações que pretende partilhar;** clique **em Guardar**.

Para obter mais informações consulte: ["A política não permite a concessão de permissões a este nível a um ou mais erros do destinatário quando o utilizador tenta partilhar o calendário](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
