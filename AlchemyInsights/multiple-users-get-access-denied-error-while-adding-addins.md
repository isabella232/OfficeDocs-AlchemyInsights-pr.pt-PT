---
title: Vários utilizadores obtêm acesso negado erro ao adicionar add-ins no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424171"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Vários utilizadores obtêm acesso negado erro ao adicionar add-ins no Outlook

Pode especificar quais os administradores da sua organização que têm permissões para instalar e gerir suplementos para o Outlook. Também pode especificar quais os utilizadores da sua organização que têm permissão para instalar e gerir suplementos para seu próprio uso.

Para mais [informações, consulte Especificar os administradores e utilizadores que podem instalar e gerir os add-ins para o Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Para verificar se atribuiu permissões a um utilizador com sucesso, <Role Name> substitua-a pelo nome da função a verificar e execute o seguinte comando no Exchange Online PowerShell:

Get-ManagementRoleAssignment - Role <Role Name> " - GetEffectiveUsers

Este exemplo mostra-lhe como verificar quem atribuiu permissões para instalar add-ins na Office Store para a organização.

PowerShell

- Papel "Org Marketplace Apps" -GetEffectiveUsers

Nos resultados, Get-ManagementRoleAssignment, reveja as entradas na coluna Utilizadores Eficazes.

Para obter informações detalhadas sobre sintaxe e [parâmetros, consulte a assinatura do Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 