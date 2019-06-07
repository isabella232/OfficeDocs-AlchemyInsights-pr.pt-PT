---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759091"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou OneDrive

Existem várias formas para restringir o acesso aos serviços do SharePoint Online/OneDrive. Estes diversos métodos de restrição de acesso são descritos abaixo. 

Restrição de permissão

No SharePoint Online e OneDrive para a empresa, vamos restringir o acesso a itens como sites, ficheiros e pastas apenas concedendo acesso aos grupos/indivíduos que deveriam ter acesso.

[Personalizar permissões para uma lista do SharePoint ou biblioteca](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Personalizar permissões do site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

[Alterar as permissões de uma subpasta](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Controlar o acesso de dispositivos não geridos](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como um SharePoint ou administrador global no Office 365, pode bloquear ou limitar o acesso ao conteúdo SharePoint e OneDrive de dispositivos não geridos (esses híbrido AD associado ou compatível no Intune).

Restrição de localização de rede

Como um administrador de TI, pode controlar o acesso a recursos do SharePoint e OneDrive com base nas localizações de rede definido que considere fidedignos. Isto também é conhecida como política baseada no local. Para mais informações, consulte [controlar o acesso ao SharePoint Online e OneDrive dados com base na localização de rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

Restrição de bloqueio de sites 

No SharePoint Online tem a capacidade para bloquear uma colecção de sites, para que ninguém tenha acesso. Isto é definido através de PowerShell e a [Shell de gestão Online do SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizando a propriedade do [Conjunto-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.

Restringir os utilizadores criem sites ou subsites

Como um administrador do SharePoint ou administrador global do Office 365, pode permitir que os utilizadores criar e administrar os seus próprios sites SharePoint, determinar que tipo de sites podem criar e especifique a localização dos sites. Para mais informações, consulte [Gerir a criação de sites no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

