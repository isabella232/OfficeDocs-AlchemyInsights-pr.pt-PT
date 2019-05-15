---
title: Site moderna, tal como o site de raiz
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057755"
---
# <a name="modern-site-as-root-site"></a>Moderno site como site de raiz

Os clientes de [Edição de destino](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) agora podem activar a experiência de site modernas de comunicação no site de raiz clássico de seu tenant do SharePoint.

Esta funcionalidade pode ser activada ao executar um cmdlet PowerShell simple. Sobre a execução com êxito do comando PowerShell, o site de raiz terá uma nova comunicação site home page. Estão disponíveis no artigo [SPOCommSite activar](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)detalhes sobre os requisitos de cmdlet e funcionalidade do PowerShell. 

Vamos vai ser gradualmente graduais este problema, desligado por predefinição, para clientes alvo Release no início de Maio de 2019, e a expandir o estarão disponível em todo o mundo até ao final de Junho de 2019. Continue a consultar o [Centro de mensagens](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) para outras funcionalidades novas com moderna. 

**Importante**: não elimine o site de raiz clássico para criar um Site de comunicação modernos. Não é suportada pela Microsoft. Eliminar o site de raiz fará com que todos os sites SharePoint da sua organização inacessíveis a todos os utilizadores, até que restaure o site ou crie um novo site com o mesmo URL. 
 
 