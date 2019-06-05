---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719527"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lenta, inacessível ou indisponível para múltiplos utilizadores

Se um site da OneDrive ou o SharePoint não está disponível para vários utilizadores, que tinham anteriormente acesso, poderá existir um problema de serviço temporária. [Verifique o dashboard de estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Adicionar e licenciar o utilizador

Certifique-se de que o utilizador [atribuir licenças aos utilizadores no Office 365 para a empresa](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Atribuir permissões

Se o utilizador tiver sido atribuído uma licença do Sharepoint e continua a receber uma mensagem de acesso negado, certifique-se de que têm o [nível de permissão adequados](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) atribuído.

## <a name="consider-using-the-access-request-feature"></a>Considere utilizar a funcionalidade de pedido de acesso

A [funcionalidade de pedido de acesso](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite às pessoas a pedir acesso ao conteúdo que não têm actualmente permissão para ver.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Permitir script personalizado pode fazer com que o acesso negado problemas

Existem determinados cenários em que a funcionalidade de *Permitir script personalizado* pode apresentar um acesso negado. Para uma lista de funcionalidades afectadas, considerações de segurança e a capacidade para desactivar a funcionalidade. Visite [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

