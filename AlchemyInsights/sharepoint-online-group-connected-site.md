---
title: Adicionar um grupo a um site do SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719492"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Criar site ligado grupo SharePoint Online

<p><strong>Existem alguns problemas comuns encontrados quando criar ou recriar um grupo de ligado o site.&nbsp;</strong></p>  <p>1.Se tiver eliminado um grupo e o respectivo site ligado e se pretende criar outro site com o mesmo URL, terá de remover permanentemente o site anterior.</p>  <ul>  <li>Transferir o <a title="SPO Shell de gestão" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Shell de gestão de SPO</a> - para obter mais informações acerca de como começar com o powershell, consulte <a title="começar a trabalhar com a Shell de gestão Online do SharePoint" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Introdução à Shell de gestão Online do SharePoint</a>. <br /><br /></li>  <li>Remover o Site Sites eliminada a utilizar o <a title="SPODeletedSite remover" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remover SPODeletedSite</a> cmdlets do powershell.</li>  </ul>  <p>Se estiver a criar um site ligado de grupo e receber um aviso <strong>'existe outro grupo com o mesmo alias já'</strong>, verifique os grupos existentes da <a title="Office 365 partir do Centro de administração" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 partir do Centro de administração</a>. Para resolver o problema, eliminar o grupo existente, se já não é necessário ou criar o site com um alias diferente atribuída.&nbsp;</p>  <p><strong>Existem diferentes formas de criar e utilizar grupos modernos com o SharePoint.&nbsp;</strong></p>  <ol>  <li>Pode ligar a sites existentes a um grupo do Office 365. Para obter mais informações, consulte <a title="ligar um grupo de Office 365 utilizando o ineterface de utilizador do SharePoint" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Ligar um grupo de Office 365 utilizando o ineterface de utilizador do SharePoint</a>.</li>  <li>Para criar um site ligado de grupo do Office 365, terá de criar um Site de equipa. Para obter mais informações, consulte <a title="criar um site de equipa do SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Crie um site de equipa do SharePoint.</a></li>  </ol>

