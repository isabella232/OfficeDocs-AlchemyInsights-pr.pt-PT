---
title: Problemas de conexão do SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727182"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de conexão do SharePoint Designer 

Se o SharePoint Designer estiver a ter problemas de ligação aos sites do SharePoint, experimente as seguintes soluções comuns.

Passo 1: Verifique se o SharePoint Designer 2013 é atualizado com o [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e a [Atualização de 2 de agosto de 2016 para o SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Passo 2: Limpar os ficheiros de cache locais:

1. Close SharePoint Designer 2013.

2. No computador local, remova todos os ficheiros encontrados em cada uma das pastas que se seguem.

    - %APPDATA%\Microsoft\Extensões do servidor web\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra o SharePoint Designer 2013 e introduza novamente a conta para ver se funciona.

Passo 3: [Ativar a autenticação moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Passo 4: Os administradores terão de **permitir scripts personalizados** nas definições do Centro de Administração SharePoint para permitir a ligação do SharePoint Designer. Consulte [Permitir ou prevenir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.


