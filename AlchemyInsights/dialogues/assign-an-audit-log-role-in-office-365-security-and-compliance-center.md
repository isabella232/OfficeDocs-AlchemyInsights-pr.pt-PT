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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526526"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="12946-102">Atribuir uma função de Registo de Auditoria no Office 365 Security & Compliance Center</span><span class="sxs-lookup"><span data-stu-id="12946-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="12946-103">Para pesquisar o registo de auditoria do Office 365, deve ser atribuído a um administrador a função **'Registos de Auditoria' view-Only** ou a função **de Registos de Auditoria** no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="12946-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="12946-104">Estas funções são atribuídas aos grupos de funções de Gestão de Conformidade e Gestão da Organização por padrão.</span><span class="sxs-lookup"><span data-stu-id="12946-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="12946-105">Os administradores globais do Office 365 e microsoft 365 são automaticamente adicionados como membros do grupo de funções de Gestão da Organização.</span><span class="sxs-lookup"><span data-stu-id="12946-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="12946-106">Para permitir que um utilizador procure com o nível mínimo de privilégios, crie um grupo de funções personalizado no Exchange Online, adicione o papel **de Registos de Auditoria Apenas ver-Apenas** ou **Funções de Registos de Auditoria** e, em seguida, adicione o utilizador como membro do novo grupo de funções.</span><span class="sxs-lookup"><span data-stu-id="12946-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="12946-107">Para obter mais informações, consulte [Gerir grupos de funções em Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) e pesquisar o registo de auditoria no Centro de Conformidade & de [Segurança.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="12946-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>