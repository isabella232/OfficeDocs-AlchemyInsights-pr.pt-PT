---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750675"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

Há muitas maneiras de restringir o acesso aos serviços do SharePoint Online/OneDrive. Esses vários métodos de restrição de acesso são descritos abaixo. 

**Restrição de permissão**

No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, arquivos e pastas apenas concedendo acesso a esses grupos/indivíduos que devem ter acesso.

- [Personalizar permissões para uma lista ou biblioteca do SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizar as permissões do site do SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alterar as permissões em uma subpasta](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não geridos](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como um administrador global ou do SharePoint no Office 365, você pode bloquear ou limitar o acesso ao conteúdo do SharePoint e do OneDrive de dispositivos não gerenciados (aqueles não híbridos AD ingressados ou compatíveis com o Intune).

**Restrição de local de rede**

Como um administrador de ti, você pode controlar o acesso aos recursos do SharePoint e do OneDrive com base em locais de rede definidos que você confia. Isso também é conhecido como política baseada em local. Para obter mais informações, consulte [controlar o acesso aos dados do SharePoint Online e do onedrive com base no local da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de bloqueio de site** 

No SharePoint Online, você tem a capacidade de bloquear um conjunto de sites, para que ninguém tenha acesso. Isso é definido por meio do PowerShell e do [Shell de gerenciamento do SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) usando a propriedade [set-soposto](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir os usuários de criar sites ou subsites**

Como administrador do SharePoint ou administrador global do Office 365, você pode permitir que seus usuários criem e administrem seus próprios sites do SharePoint, determinem que tipo de sites eles podem criar e especifique o local dos sites. Para obter mais informações, consulte [gerenciar a criação de site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

