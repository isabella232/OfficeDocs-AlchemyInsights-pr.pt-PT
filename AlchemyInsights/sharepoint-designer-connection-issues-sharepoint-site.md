---
title: Problemas de conexão sharepoint designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051724"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de conexão sharepoint designer 

Se o SharePoint Designer está enfrentando problemas de conexão com sites do SharePoint, tente as seguintes soluções comuns.

Etapa 1: Verifique se o SharePoint Designer 2013 é atualizado com o Pacote de Serviço de [Designer SharePoint 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e a atualização de 2 de agosto de [2016 para designer sharepoint 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Passo 2: Limpe os arquivos de cache locais:

1. Fechar SharePoint Designer 2013.

2. No computador local, remova todos os arquivos encontrados em cada uma das seguintes pastas.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\Web Server Extensões \Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra sharepoint designer 2013 e digite a conta novamente para ver se ele funciona.

Etapa 3: [Habilite autenticação moderna para o Office 2013 em dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Passo 4: Os administradores precisarão **permitir o script personalizado** nas configurações do SharePoint Admin Center para permitir a conexão SharePoint Designer. Veja [permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.


