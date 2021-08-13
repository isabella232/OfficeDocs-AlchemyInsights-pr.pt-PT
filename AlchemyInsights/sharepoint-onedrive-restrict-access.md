---
title: Restringir o acesso no SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093849"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou OneDrive

Existem várias formas de restringir o acesso ao SharePoint Online/OneDrive serviços. Estes vários métodos de restrição de acesso estão indicados abaixo. 

**Restrição de Permissão**

No SharePoint Online e no OneDrive para Empresas, restringimos o acesso a itens como sites, ficheiros e pastas ao conceder apenas acesso aos grupos/pessoas que devem ter acesso.

- [Personalizar permissões para uma lista ou biblioteca do SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizar permissões de site do SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alterar as permissões numa subpata](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não geridos](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como administrador global ou do SharePoint, pode bloquear ou limitar o acesso ao SharePoint e OneDrive conteúdos de dispositivos não manterados (os que não estão associados ou em compatibilidade com o AD híbrido no Intune).

**Restrição de Localização de Rede**

Enquanto administrador de TI, pode controlar o acesso a recursos do SharePoint OneDrive com base em localizações de rede definidas das suas confiança. Isto também é conhecido como política baseada na localização. Para obter mais informações, consulte Controlar [o acesso ao SharePoint Online e OneDrive dados com base na localização de rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de Bloqueio de Site** 

No SharePoint Online tem a capacidade de bloquear uma coleção de site, para que ninguém tenha acesso. Isto é definido através do PowerShell e da Shell de Gestão do [SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) com a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir a criação de sites ou subsites por parte dos utilizadores**

Como administrador do SharePoint ou Administrador global, pode permitir que os seus utilizadores criem e administram os respetivos sites do SharePoint, determinar o tipo de sites que podem criar e especificar a localização dos sites. Para obter mais informações, consulte Gerir [a criação de site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

