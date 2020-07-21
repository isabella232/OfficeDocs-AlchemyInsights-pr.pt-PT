---
title: Vários utilizadores que não vêem add-ins no Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198238"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Vários utilizadores que não vêem add-ins no Outlook

Se testar os add-ins do Outlook e nenhum aparecer, como um primeiro passo de resolução de problemas, utilize o cmdlet **Get-OrganizationConfig** PowerShell para consultar o parâmetro _AppsForOfficeEnabled._ Se a consulta devolver um valor de **Falso,** desafie este parâmetro para **True** utilizando o **cmdlet Set-OrganizationConfig,** para que os add-ins apareçam como esperado.

Não recomendamos que o parâmetro _AppsForOfficeEnabled_ esteja definido como **Falso**. Um valor de **Falso** sobrepõe-se a todas as definições de funções administrativas e de utilizador acima e impede que quaisquer novas aplicações sejam ativadas por qualquer utilizador da organização.

Para obter mais informações, consulte [Especificar os administradores e utilizadores que podem instalar e gerir os add-ins para o Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).