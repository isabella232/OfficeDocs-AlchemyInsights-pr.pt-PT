---
title: Restringir o acesso no SharePoint ou oneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692776"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou oneDrive

Existem muitas formas de restringir o acesso aos serviços SharePoint Online/OneDrive. Estes vários métodos de restrição de acesso são descritos abaixo. 

**Restrição de Permissão**

No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, ficheiros e pastas, concedendo apenas acesso aos grupos/indivíduos que deveriam ter acesso.

- [Personalize permissões para uma lista de SharePoint ou biblioteca](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalizar permissões do site do SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alterar as permissões numa subpasta](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não geridos](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como um SharePoint ou administrador global, pode bloquear ou limitar o acesso ao conteúdo sharePoint e OneDrive a partir de dispositivos não geridos (aqueles que não são a D.C. híbridos unidos ou conformes no Intune).

**Restrição de Localização da Rede**

Como administrador de TI, pode controlar o acesso aos recursos SharePoint e OneDrive com base em localizações de rede definidas em que confia. Isto também é conhecido como política baseada na localização. Para mais informações, consulte [o acesso do Controlo aos dados SharePoint Online e OneDrive com base na localização da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de bloqueio do site** 

Dentro do SharePoint Online tem a capacidade de bloquear uma coleção de site, para que ninguém tenha acesso. Isto é definido através da PowerShell e da [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizando a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir os utilizadores à criação de sites ou subsites**

Como administrador do SharePoint ou administrador global, pode permitir que os seus utilizadores criem e administram os seus próprios sites SharePoint, determinem que tipo de sites podem criar e especificar a localização dos sites. Para mais informações, consulte Gerir a criação do [site no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

