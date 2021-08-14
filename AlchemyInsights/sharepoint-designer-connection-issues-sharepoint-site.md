---
title: Problemas de ligação do SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942036"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de ligação do SharePoint Designer 

Se o SharePoint Designer estiver com problemas de ligação a sites do SharePoint, experimente as seguintes soluções comuns.

Passo 1: verifique se o SharePoint Designer 2013 é atualizado com o [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e a Atualização de 2 de agosto de [2016 para o SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Passo 2: Limpar os ficheiros de cache locais:

1. Feche o SharePoint Designer 2013.

2. No computador local, remova todos os ficheiros encontrados em cada uma das seguintes pastas.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra o SharePoint Designer 2013 e introduza a conta novamente para ver se funciona.

Passo 3: [Ativar a Autenticação Moderna Office 2013 em Windows Dispositivos](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Passo 4: os administradores terão de Permitir **Script** Personalizado nas definições do Centro de Administração do SharePoint para permitir a ligação ao SharePoint Designer. Consulte [Permitir ou impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.


