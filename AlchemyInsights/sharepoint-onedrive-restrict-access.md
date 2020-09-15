---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700466"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

Existem muitas formas de restringir o acesso aos serviços SharePoint Online/OneDrive. Estes vários métodos de restrição de acesso são descritos abaixo. 

**Restrição de Permissão**

No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, ficheiros e pastas, concedendo apenas acesso a esses grupos/indivíduos que deveriam ter acesso.

- [Personalize permissões para uma lista ou biblioteca sharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalize permissões do site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Altere as permissões numa sub-dobra](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não geridos](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como administrador do SharePoint ou global, pode bloquear ou limitar o acesso ao conteúdo sharePoint e OneDrive a partir de dispositivos não geridos (aqueles que não são híbridos ad joined ou compliant in Intune).

**Restrição de localização da rede**

Como administrador de TI, pode controlar o acesso aos recursos sharePoint e OneDrive com base em localizações de rede definidas em que confia. Isto também é conhecido como política baseada na localização. Para mais informações, consulte [o acesso ao Control para os dados do SharePoint Online e do OneDrive com base na localização da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de bloqueio do site** 

No SharePoint Online tem a capacidade de bloquear uma coleção de sites, para que ninguém tenha acesso. Isto é definido através do PowerShell e da [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizando a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir os utilizadores da criação de sites ou subsites**

Como administrador do SharePoint ou administrador global, pode permitir que os seus utilizadores criem e administram os seus próprios sites SharePoint, determinem que tipo de sites podem criar e especificar a localização dos sites. Para mais informações, consulte [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

