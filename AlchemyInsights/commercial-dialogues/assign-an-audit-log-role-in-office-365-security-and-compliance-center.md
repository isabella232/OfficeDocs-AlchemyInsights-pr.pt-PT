---
title: Atribuir uma função de Registo de Auditoria no Office 365 Security & Compliance Center
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749519"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Atribuir uma função de Registo de Auditoria no Office 365 Security & Compliance Center

Para pesquisar o registo de auditoria do Office 365, deve ser atribuído a um administrador a função **'Registos de Auditoria' view-Only** ou a função **de Registos de Auditoria** no Exchange Online. Estas funções são atribuídas aos grupos de funções de Gestão de Conformidade e Gestão da Organização por padrão. Os administradores globais do Office 365 e microsoft 365 são automaticamente adicionados como membros do grupo de funções de Gestão da Organização.

Para permitir que um utilizador procure com o nível mínimo de privilégios, crie um grupo de funções personalizado no Exchange Online, adicione o papel **de Registos de Auditoria Apenas ver-Apenas** ou **Funções de Registos de Auditoria** e, em seguida, adicione o utilizador como membro do novo grupo de funções.

Para obter mais informações, consulte [Gerir grupos de funções em Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) e pesquisar o registo de auditoria no Centro de Conformidade & de [Segurança.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)