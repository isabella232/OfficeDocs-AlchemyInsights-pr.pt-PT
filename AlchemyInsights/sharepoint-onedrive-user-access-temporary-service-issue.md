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
ms.openlocfilehash: 880b2bdd7b74f4365bcbff73a709d42e72be0e3a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36535186"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lenta, inacessível ou indisponível para múltiplos utilizadores

Se um site da OneDrive ou o SharePoint não está disponível para vários utilizadores, que tinham anteriormente acesso, poderá existir um problema de serviço temporária. [Verifique o dashboard de estado de funcionamento do serviço](https://portal.office.com/adminportal/home#/servicehealth).

**Adicionar e licenciar o utilizador**

Certifique-se de que o utilizador [atribuir licenças aos utilizadores no Office 365 para a empresa](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Atribuir permissões**

Se o utilizador tiver sido atribuído uma licença do Sharepoint e continua a receber uma mensagem de acesso negado, certifique-se de que têm o [nível de permissão adequados](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.

**Considere utilizar a funcionalidade de pedido de acesso**

A [funcionalidade de pedido de acesso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite às pessoas a pedir acesso ao conteúdo que não têm actualmente permissão para ver.

**Permitir script personalizado pode fazer com que o acesso negado problemas**

Existem determinados cenários em que a funcionalidade de *Permitir script personalizado* pode apresentar um acesso negado. Para uma lista de funcionalidades afectadas, considerações de segurança e a capacidade para desactivar a funcionalidade. Visite [Permitir ou impedir que o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

