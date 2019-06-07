---
title: Níveis de permissão SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760703"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de ligação do SharePoint Designer 

Se o SharePoint Designer está com problemas de ligação aos SharePoint sites, tente as seguintes soluções comuns.

Passo 1: Verificar se o SharePoint Designer é actualizado.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [O SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Actualização para o SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Passo 2: Limpar os ficheiros de local cache

- Feche o SharePoint Designer 2013.

- No computador local, procure as seguintes pastas para remover ficheiros em cache.

- Clique em Iniciar, executar e eliminar todos os ficheiros encontrados em cada um a seguir localizações.

Servidor de %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Abra o SharePoint Designer 2013 e introduza a conta novamente para verificar se funciona.

Passo 3: [Activar a autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Passo 4: Os administradores serão necessário permitir Script personalizado para permitir a ligação do SharePoint Designer.

Para obter passos detalhados, exemplos e considerações consulte [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


