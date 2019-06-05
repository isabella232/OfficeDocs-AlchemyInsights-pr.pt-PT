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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716902"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de ligação do SharePoint Designer 

<p>Se o SharePoint Designer está com problemas de ligação aos SharePoint sites, tente as seguintes soluções comuns.</p> <p><strong>Passo 1:</strong> <strong>Verifique se o SharePoint Designer é actualizado&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">O SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Actualização para o SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Passo 2:</strong> <strong>Limpar os ficheiros de local cache</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Feche o SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">No computador local, procure as seguintes pastas para remover ficheiros em cache.&nbsp;</li> <li style="font-weight: 400;">Clique em <strong>Iniciar -&gt; executar</strong> e elimine todos os ficheiros encontrados em cada uma da seguir localizações.&nbsp;<br /><br />%APPDATA%\Microsoft\Web server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Abra o SharePoint Designer 2013 e introduza a conta novamente para verificar se funciona.</li> </ol> <p><strong>Passo 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide">De <strong>Activar a autenticação moderna para 2013 do Office em dispositivos do Windows</strong></a>&nbsp;</p> <p><strong>Passo 4:</strong> <strong>Os administradores terão de permitir Script personalizado para permitir a ligação do SharePoint Designer</strong>.</p> <p>Para obter passos detalhados, exemplos e considerações consulte <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Permitir ou impedir que o script personalizado</a>.&nbsp;</p>


