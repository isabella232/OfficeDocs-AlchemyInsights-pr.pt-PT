---
title: Adicione um grupo a um site do SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582822"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemas ao criar um site conectado a grupo no SharePoint

1. Algumas questões comuns encontradas ao criar ou recriar um site conectado a grupo.
Se eliminou um grupo e o seu site conectado e deseja criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.

   - Baixar [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Para obter mais informações sobre como começar com a Powershell, consulte [Começar com a SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Remova o Site de Sites eliminados utilizando o [cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. A Powershell é necessária para eliminar permanentemente os sites de grupo.

1. Se estiver a criar um site ligado ao grupo e receber um aviso: Outro grupo com o mesmo pseudónimo já existe , verifique os **grupos**existentes do [centro de administração Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Para resolver o problema, elimine o grupo existente se já não for necessário ou crie o site com um pseudónimo diferente atribuído.

1. Existem diferentes formas de criar e usar grupos modernos com o SharePoint.

   - Pode ligar os sites existentes a um grupo Microsoft 365. Para obter mais informações, consulte [Conecte um grupo Microsoft 365 utilizando a interface de utilizador do SharePoint.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Para criar um site ligado ao grupo Microsoft 365, terá de criar um [Site de Equipa](https://admin.microsoft.com/sharepoint).
