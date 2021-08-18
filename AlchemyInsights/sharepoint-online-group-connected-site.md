---
title: Adicionar um grupo a um site do SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897727"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemas comuns ao criar um site ligado a um grupo no SharePoint

1. Se eliminou um grupo e o seu site ligado e pretender criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.

   - Transferir Shell [de Gestão do SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Para obter mais informações sobre como começar a trabalhar com o PowerShell, consulte o trm está a começar a Trabalhar com a Shell de [Gestão do SharePoint Online.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Remova o Site de Sites Eliminados com o cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) do PowerShell. O PowerShell é necessário para eliminar permanentemente sites de grupo.

1. Se estiver a criar um site ligado a um grupo e receber um aviso: Outro grupo com o mesmo **alias** já existe, verifique os grupos existentes no centro de administração do Microsoft 365 [.](https://admin.microsoft.com/AdminPortal/Home#/groups) Para resolver o problema, elimine o grupo existente se este já não for necessário ou crie o site com um alias diferente atribuído.

1. Existem diferentes formas de criar e utilizar grupos modernos com o SharePoint.

   - Pode ligar sites existentes a um Microsoft 365 grupo. Para mais informações, consulte o [Ligação um Microsoft 365 utilizando a interface de utilizador do SharePoint.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Para criar um Microsoft 365 de grupo ligado, terá de criar um [Site de Equipa.](https://admin.microsoft.com/sharepoint)
