---
title: Restringir o acesso no SharePoint ou no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053776"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir o acesso no SharePoint ou no OneDrive

Há muitas maneiras de restringir o acesso aos serviços SharePoint Online/OneDrive. Estes vários métodos de restrição de acesso são descritos abaixo. 

**Restrição de permissão**

No SharePoint Online e no OneDrive for Business, restringimos o acesso a itens como sites, arquivos e pastas, concedendo apenas acesso a esses grupos/indivíduos que devem ter acesso.

- [Personalize as permissões para uma lista ou biblioteca do SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Personalize as permissões do site SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alterar as permissões em uma subfoldera](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Controlar o acesso de dispositivos não geridos](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Como um SharePoint ou administrador global no Office 365, você pode bloquear ou limitar o acesso ao conteúdo SharePoint e OneDrive de dispositivos não gerenciados (aqueles que não são AD híbridos se juntaram ou estiverem em conformidade em intune).

**Restrição de localização da rede**

Como administrador de TI, você pode controlar o acesso aos recursos do SharePoint e do OneDrive com base em locais de rede definidos em que você confia. Isso também é conhecido como política baseada em localização. Para mais informações, consulte o [acesso ao Controle aos dados do SharePoint Online e do OneDrive com base na localização da rede](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Restrição de bloqueio do site** 

Dentro sharepoint on-line você tem a capacidade de bloquear uma coleção do site, para que ninguém tenha acesso. Isso é definido via PowerShell e o [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) usando a propriedade [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Restringir os usuários de criar sites ou subsites**

Como administrador do SharePoint ou administrador global do Office 365, você pode permitir que seus usuários criem e administrem seus próprios sites do SharePoint, determinar que tipo de sites eles podem criar e especificar a localização dos sites. Para mais informações, [consulte a criação do site gerenciar no SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

