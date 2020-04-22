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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642155"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemas ao criar um site ligado ao grupo no SharePoint

1. Algumas questões comuns encontraram-se ao criar ou recriar um site ligado ao grupo.
Se tiver eliminado um grupo e o seu site conectado e pretender criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.

   - Baixar [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Para mais informações sobre começar com a Powershell, consulte [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Remova o Site dos Sites Eliminados utilizando o cmdlet [remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. A Powershell é necessária para eliminar permanentemente os sites do grupo.

1. Se estiver a criar um site ligado ao grupo e receber um aviso: **Outro grupo com o mesmo pseudónimo já existe,** verifique os grupos existentes do Microsoft [365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Para resolver o problema, elimine o grupo existente se já não for necessário ou criar o site com um pseudónimo diferente atribuído.

1. Existem diferentes formas de criar e usar grupos modernos com o SharePoint.

   - Pode ligar os sites existentes a um grupo do Office 365. Para mais informações, consulte [Connect um grupo Office 365 utilizando a interface de utilizador do SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Para criar um site ligado ao grupo Office 365, terá de criar um Site de [Equipa.](https://admin.microsoft.com/sharepoint)
