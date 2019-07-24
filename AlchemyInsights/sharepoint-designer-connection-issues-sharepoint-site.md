---
title: Problemas de ligação do SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840562"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de ligação do SharePoint Designer 

Se o SharePoint Designer está com problemas de ligação aos SharePoint sites, tente as seguintes soluções comuns.

Passo 1: Verificar se o SharePoint Designer 2013 é actualizado com o [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e [2 de Agosto de 2016 actualização para o SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Passo 2: Limpe os ficheiros de local cache:

1. Feche o SharePoint Designer 2013.

2. No computador local, remova todos os ficheiros localizados em cada uma das seguintes pastas.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra o SharePoint Designer 2013 e introduza a conta novamente para verificar se funciona.

Passo 3: [Activar a autenticação moderna para 2013 do Office em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Passo 4: Os administradores serão necessário **Permitir Script personalizado** nas definições do Centro de administração do SharePoint para permitir a ligação do SharePoint Designer. Consulte [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.


