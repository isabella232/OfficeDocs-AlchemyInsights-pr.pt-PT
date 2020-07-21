---
title: Único utilizador que não vê add-ins no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198216"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Único utilizador que não vê add-ins no Outlook

O utilizador pode fazer parte de uma função que não tem o parâmetro AppsForOfficeEnabled correto. Executar este cmdlet para saber se a função correta está associada ao utilizador:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false [ Formato-Tabela - Função Automática,RoleAssigneeName,RoleAssigneeType

Para obter mais informações, consulte [Especificar os administradores e utilizadores que podem instalar e gerir os add-ins para o Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
