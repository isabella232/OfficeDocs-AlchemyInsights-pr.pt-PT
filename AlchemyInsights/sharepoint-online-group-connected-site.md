---
title: Adicionar um grupo a um site do SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750531"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemas durante a criação ou de grupo ligado a sites SharePoint Online

Existem alguns problemas comuns encontrados quando criar ou recriar um grupo de ligado o site.

 Se tiver eliminado um grupo e o respectivo site ligado e se pretende criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.

Transferir a [Shell de gestão de SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Para obter mais informações acerca de como começar com o powershell, consulte [Introdução à Shell de gestão Online do SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Remova o Site de Sites eliminada utilizando o cmdlet de powershell [Remover SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Se estiver a criar um site ligado de grupo e receber um aviso de que outro grupo com o mesmo alias já existe, verifique os grupos existentes do [Office 365 partir do Centro de administração](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Para resolver o problema, eliminar o grupo existente, se já não é necessário ou criar o site com um alias diferente atribuída.

Existem diferentes formas de criar e utilizar grupos modernos com o SharePoint.

Pode ligar a sites existentes a um grupo do Office 365. Para obter mais informações, consulte [ligar um grupo de Office 365 utilizando o ineterface de utilizador do SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Para criar um site ligado de grupo do Office 365, terá de criar um Site de equipa. Para obter mais informações, consulte [criar um site de equipa do SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

