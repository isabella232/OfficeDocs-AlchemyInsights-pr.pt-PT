---
title: Eliminar permanentemente um site no SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944322"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Eliminar permanentemente um site no SharePoint

Para reutilizar um URL de um site eliminado (para recriar um site) ou para eliminar permanentemente um site porque o mesmo já não está a ser utilizado, pode utilizar a opção **Eliminar Permanentemente** a partir do Novo Centro de Administração do SharePoint. 

1. Aceda a [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) (Página de sites eliminados do novo centro de administração do SharePoint) e inicie sessão com uma conta que tenha permissões de administrador para a sua organização. 

2. Na coluna da esquerda, selecione um site. 

3. Clique em **Eliminar Permanentemente**. 

**Nota**: os sites conectados em grupo não podem ser eliminados permanentemente do Novo Centro de Administração do SharePoint. Será necessário utilizar o [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Para mais informações, consulte [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) (Eliminar permanentemente um site). 
