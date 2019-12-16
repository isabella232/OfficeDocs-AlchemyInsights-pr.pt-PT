---
title: Adicionar um grupo a um site do SharePoint
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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051112"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemas ao criar ou agrupar sites conectados no SharePoint Online

Há um par de problemas comuns encontrados ao criar ou recriar um site conectado em grupo.

 Se você excluiu um grupo e seu site conectado e deseja criar outro site com a mesma URL, você precisará remover permanentemente o site anterior.

Baixe [o Shell de gestão SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Para mais informações sobre como começar com powershell, veja [começar com sharepoint online management shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Retire o site de sites excluídos usando o cmdlet de casca de potência [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Se você está criando um site conectado em grupo e receber um aviso Outro grupo com o mesmo pseudônimo já existe, verifique os grupos existentes do [Office 365 do Centro de Administração.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups) Para resolver o problema, exclua o grupo existente se ele não for mais necessário ou criar o site com um pseudônimo diferente atribuído.

Existem diferentes maneiras de criar e usar grupos modernos com sharepoint.

Você pode conectar sites existentes a um grupo do Office 365. Para mais informações, [consulte o grupo Connect an Office 365 usando o ineterface do usuário Do SharePoint.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)

Para criar um site conectado ao grupo Office 365, você precisará criar um site de equipe. Para mais informações, consulte criar um site de [equipe no SharePoint.](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)

